Rubricoin Tokens
===========

The Rubric Service Network (RSN) uses tokens callled rubricoins for all internal transactions.

* Storage fees are calculated in rubricoins
* Rubric owners are reimbused for their services in rubricoins
* Object transfer fees are paid in rubricoin
* Rubric Compute Container (RCC) fees are paid in rubricoin

Accounting
------------------

Example Scenario
-----------------------------
A Rubric Client (RC) wants to store a Rubroic Object (RO) for one year so they contratc with a Rubric (R) for that service.
To make math easy we'll say its a large file and it will cost 365 Rubricoin (RBC) to store the RO for one year.

### Transaction Process 
1. The RC provides the RO and 365 RBC to the Rubric.
    Those 365 RBC are in an encumbered transaction so there are really 365 "encumbered RBC" (eRBC).
2. The Rubric accepts the transaction and stores the file.
3. Each day at midnight GMT 1 RBC becomes un-emcumbered and can be spent by the Rubric.

### Normal Fulfillment 
The normal fulfillment would be that the Rubric store the object for one year and then create a transaction that includes the RO and sends the now unemcumberd RBC to an address chosen by the RC. the RSN requires that Rubric include the RO in the spend transaction even after the encumbrance has expired is done as a way to verify that the Rubric did mantain a copy of the RO the entire time.


### Spending the eRBC 
For the sake of our exampe we'll say that 40 days into the contract the Rubric wants to use the 40 RBC that have become unencumbered. The RSN needs to ensure that the remain 325 eRBC are stilled tied to the obligation to store the RO.

*Scenario 1 - Rubric retains contract*

If the Rubric is willing to continue storing the RO they can spend the encumbered transaction sending the 40 unencumbered RBC to and address of their choosing and the encumbered change back to their address. 

The RSN needs to ensure that the Rubric is still storing the RO before recording the transaction. If not the Rubric could take the contract and immediately delete te fiel to save themselves the cost of storing it. Then on day 364 of the contract they could spend 364 of the 365 RBC provided by the RC. Then if on day 365 the RC request the RO it won't exist, the 1 remaining eRBC is going to provide little solace to the RC.

*Scenario 2 - Rubric transfers contract*

If the Rubric is unwilling to continue storing the RO they must transfer the obejct and the remaining eRBC to a Rubric willing to fulfill the remainder of the contract.

The creator of the RO may have added an additional encumbrance that their signature is required for any early spends of the transaction where the eRBC goes to anyone other than the original  Rubric. This would allow them to ensure thatb they beleived the new Rubric would be able to provide all the required services.  

*Scenario 3 - Rubric deletes the file*

If the RSN enforces that the correct RO is provided when spending any
