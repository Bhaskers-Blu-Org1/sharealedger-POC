# Sharealedger-POC
This respository contains historical information about work on Sharealedger.org.

The work has been promoted to a separate Open Source Project visible at https://github.com/sharealedger-org/sharealedger and at http://sharealedger.org.

# Scalable Architecture for Financial Reporting

Much of the work of creating ledgers at scale comes from IBM's Scalable Architecture for Financial Reporting (SAFR).  You can read more about it here:  http://www.redbooks.ibm.com/abstracts/REDP4599.html?Open


# Really Simple Commerce

The earliest work is documented in https://github.com/KipTwitchell/VAPostAnalysisRSCDemo

This system has three major parts to

A posting engine process
A simple analysis engine
A simple data capture engine
A simple join program, called Match-Merge

The Posting and Analysis Engines demonstrate what historical ledger functions at scale.  
The match-merge is a drill down on one type of process which provides scale to the system with great efficiencies.
The Really Simple Commerce (RSC) component provided an approach for shared commerce over very simple means but with the added benefit of a fully functional ledger behind the system.

The system simulates three terminal screens can be used to present an interactive text messaging system between the server and three other parties:
1. The Authorizer can add a new Customer (2) to the the RSC network.
2. The Customer can accept invitations to join the network, can add details to their customer records, and can pay for goods and services when invited by the (3) vendor
3. The Vendor specifies amounts for the customer to pay, and accepts payment.

It combines payment, shared ledgers, democratization of credit creation, social network, and may ultimately extend to virtual currencies. The transaction capture outputs from such a system would be posted into a universal ledger, that would provide the on-going control for the members of the community.

The system does not use cell phone values, and there are no edits on the input data.  The state of each cell phone must be waiting for response from the server before the server sends that response or the system hangs.  The system uses named pipes to communicate to each other in their respective roles.  No two terminal can share the same role at the same time.  The data in this part of the system is not connected to the VA data used in the other two parts of the system.

# z/OS Related Projects

SAFR's exploitation of z/OS has led to other POC efforts, which are not yet released as Open Source. The use of more modern languages on z can be read about in this blog entry: https://ledgerlearning.com/2020/03/26/scala-on-z/

Other projects will be released with time.    