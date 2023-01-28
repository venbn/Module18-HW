# PyChain Ledger

![alt=""](Images/application-image.png)

You’re a fintech engineer who’s working at one of the five largest banks in the world. You were recently promoted to act as the lead developer on their decentralized finance team. Your task is to build a blockchain-based ledger system, complete with a user-friendly web interface. This ledger should allow partner banks to conduct financial transactions (that is, to transfer money between senders and receivers) and to verify the integrity of the data in the ledger.

You’ll make the following updates to the provided Python file for this assignment, which already contains the basic `PyChain` ledger structure that you created throughout the module:

1. Create a new data class named `Record`. This class will serve as the blueprint for the financial transaction records that the blocks of the ledger will store.

2. Modify the existing `Block` data class to store `Record` data.

3. Add Relevant User Inputs to the Streamlit interface.

4. Test the PyChain Ledger by Storing Records.

---
## Files

Download the following files to help you get started:

[Module 18 Homework files](Starter_Code/pychain.py)

---

## Introduction

This project is to build an Ledger application using PyChain module which records the transactions and tag them with a unique hash value.

### Step 1: Create a Record Data Class

Added a new class called `Record` within the `@dataclass` decorator and add 3 attributes `sender`, `receiver` and `amount`.

Note that you’ll use this new `Record` class as the data type of your `record` attribute in the next section.

### Step 2: Modify the Existing Block Data Class to Store Record Data

Renamed `data` attribute in `Block` class to `record` which will use the new instance of `Record` class.

### Step 3: Add Relevant User Inputs to the Streamlit Interface

Deleted `input_data` variable from the streamlit interface and added input areas for `sender`, `receiver` and `amount` attributes so that inputs are accepted on the streamlit front-end application.

Added an "Add Block" button which will pickup the transaction information in the form of `record` from the `new_block`, stores the transactions, generates/tags the unique hash value (representing mined blocks) and displays them in the ledger format on the web page.

### Step 4: Test the PyChain Ledger by Storing Records

The `PyChain` ledger user interface has been testing by executing the `pychain.py` code using Streamlit application, the testing process will record the transactions and validates the blockchain.

The ledger has been tested by performing several transactions which does the following

    - Provide inputs for sender, receiver and amount attributes several times and stores/displays the blocks 
    - Verify the block contents and hashes in the Streamlit dropdown menu. 

Below is the Screenshot of the streamlit application page has been taken which records the multiple transactions and blocks :

[](PyChainLedger.mp4)


---
