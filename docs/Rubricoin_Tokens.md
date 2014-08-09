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

=== Transaction Process ===
1. The RC provides the RO and 365 RBC to the Rubric.
    Those 365 RBC are in an encumbered transaction so there are really 365 "encumbered RBC" (eRBC).
2. The Rubric accepts the transaction and stores the file.
3. Each day at midnight GMT 1 RBC becomes un-emcumbered and can be spent by the Rubric.

==== Normal Fulfillment ===
The normal fulfillment would be that the Rubric store the object for one years and then when the transaction's encumbrance expires the Rubric can spend or transfer the full 365 RBC.
The only thing that needs to be accounted for here is what to do if the Rubric failed to respond to request for that object within that time. 

=== Spending the eRBC ===
For the sake of our exampe we'll say that 40 days into the contract the Rubric wants to use the 40 RBC that have become unencumbered. The RSN needs to ensure that the remain 325 eRBC are stilled tied to the obligation to store the RO.



