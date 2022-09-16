# words-chain
Wordle Clone enabled for web3


What makes it interesting?
  Unlimited Play - select word(s) using VRF (Verifiable Random Function)
  			from Chainlink
  Save your results on-chain
  Using the VRF to select the words will allow games of multiple words
  Invite friends to play multiple sets of words competitively
   (using the same Random seed), makes it hard to cheat.

  Parameters for multi-player game.
  	1) Number of players
  	2) Number of words in game
  	3) Time limit to complete
  	4) Select prize (NFT, or entrance fees to winner)

  The person that wants to set up the game, connects to web3 wallet,
  sets up the game parameters, and invites players to the game.  
  Invited players join the game with their web3 wallets and put 
  token(s) into the contract.
  When number of players has been satisfied, random number is provided by Chainlink VRF.  Each player is presented with the same set of words.
  The competition is scored by 
    1) number of words solved
    2) (if tied) attempts per word
    3) (if tied) elapsed time
  When all participants have completed the game, (or timed out using a Chainlink keeper), winner is determined, NFT of the game is generated and shipped to the winner along with the tokens entered in to the contract.

  The elements of web3:
    smartcontract controls game entry and exit
    VRF is used to select words to prevent cheating
    Keeper is used to end game if not all players finish
    IPFS is used to store the words database
    smartcontract 
    	1) generates ERC-721 NFT with game data
    	2) reward from entrance fees is calculated 
    	3) allows only winner to claim the 'prizes'

    


