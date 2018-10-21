Security Organizations
=========================

The following information is always in draft status and should be used as a guide. If you are a security professional, please join our research and contribute to our ongoing effort!

## Risk Associated Questions to Consider   

The associated risk (potential threat level) of a smart contract will dictate the level of auditing it needs to go through. Here are a few questions you can ask yourself to ascertain its associated risk level:

1. Does it control funds?
2. Are official decisions derived from it?
3. What potential network effect impacts could it have?
    * network congestion
    * associated costs of usability depending on current network congestion
    * Examples in the wild to learn from?   

## Levels of Auditing   

Once you have figured out the risk of a given smart contract, then you can decide what type of auditing it should go through for deployment.   

  * Internal Review - within working group   
  * Internal Review - including internal auditor outside working group   
  * 1 round of external 3rd party auditing   
  * $n$ rounds of external 3rd party auditing   

## Topics to be Audited   

Here is a list of topics to be aware of when performing audits:   

  * Unit tests passing
  * Compilator warnings
  * Race Conditions. Reentrancy. Cross-function Race Conditions. Pitfalls in Race Condition solutions
  * Transaction-Ordering Dependence (front running)
  * Timestamp Dependence
  * Integer Overflow and Underflow
  * DoS with (unexpected) Revert
  * DoS with Block Gas Limit
  * Methods execution permissions
  * Oracles calls
  * Private user data leaks
  * Forcibly sending ether to a contract
  * Ownership of the deployed contract
