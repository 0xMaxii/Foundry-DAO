# Foundry DAO project

1. We are going to have a contract controlled by a DAO
2. Every transaction that the DAOwants to send has to be voted on
3. We will use ERC20 tokens for voting 

The Openzeppelin Wizard has a total different content and it misses this import inside GovToken.sol: import {Nonces} from "@openzeppelin/contracts/utils/Nonces.sol";

The voting delay has now changed from 1 block to 7400: this value has to be updated also for the VOTING_DELAY state variable inside GovernorTest.sol.
