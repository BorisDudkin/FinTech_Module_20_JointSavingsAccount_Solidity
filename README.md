# Joint Savings Account Smart Contract

### The Cryptocurrency Payments Solution allows a user to make ETH denominated payments to individuals, who have an ETH account (and address). The application is equiped with a user-friendly web interface that provides a functionality to veiw the user's ETH balance, select individuals for making payments, apply the hours of their service and calculate the corresponding amount of ETH transfer and, finally, send a payment and verify the transaction.

---

![crypto](Images/joint.jpg)

---

## Table of contents

1. [Technologies](#technologies)
2. [Installation Guide](#installation-guide)
3. [Usage](#usage)
4. [Contributors](#contributors)
5. [License](#license)

---

## Technologies

`Python 3.9`

_Libraries_

1. `Pandas` is a Python package that provides fast, flexible, and expressive data structures designed to make working with large sets of data easy and intuitive.

   - [pandas](https://github.com/pandas-dev/pandas) - for the documentation, installation guide and dependencies.

2. `Streamlit` is a library that allows developers to build web applications with live user input.

   - [Streamlit](https://streamlit.io/) - to read more about deploying, installing and customizing.<br/>

3. `Web3.py` is a Python library for connecting to and performing operations on Ethereum-based blockchains.

   - [Web3.py](https://web3py.readthedocs.io/en/stable/overview.html) - to get a sense of everything web3.py can do and to serve as a quick reference guide, including a summary of each feature with links to learn more.

4. `Mnemonic` is a Python library that provides access to the tools we’ll use to test Ethereum-based applications.

   - [Mnemonic](https://pypi.org/project/mnemonic/) - to read about the implementation of a mnemonic code or mnemonic sentence – a group of easy to remember words – for the generation of deterministic wallets.

5. `Bip44` is a Python implementation for deriving hierarchical deterministic wallets from a seed phrase based on the BIP-44 standard.

   - [Bip44](https://pypi.org/project/bip44/) - to read about the installation and a quick start.

6. `Ganache` is a program that allows you to quickly set up a local blockchain, which you can use to test and develop smart contracts.

   - [Ganache](https://trufflesuite.com/ganache/) - to read about the installation and the initiation of the program.

---

## Installation Guide

The application must be started from the terminal using Streamlit, once in the directory of the application:<br/>

```python
streamlit run fintech_finder.py
```

### Library Installations

Before using the application first install the following dependencies by using your terminal:

> Option 1 - Intsall needed libraries with requirements.txt file included in the reporsitory. For this option:<br/>

- install [pipreqs](https://pypi.org/project/pipreqs/):

  ```python
  pip install pipreqs
  ```

- Install all libraries that we have in requirements.txt::

  ```python
  pip install -r requirements.txt:
  ```

> Option 2 - Install each library individually:<br/>

To install pandas run:

```python
pip install pandas
```

```python
# or conda
conda install pandas
```

To install Streamlit, in Terminal run:

```python
pip install streamlit
```

Confirm the installation of the Streamlit package by running the following commands in Terminal:

```python
 conda list streamlit
```

To install Web3.py, in Terminal run:

```python
pip install web3==5.17
```

To install Mnemonic, in Terminal run:

```python
pip install mnemonic
```

To install Bip44, in Terminal run:

```python
pip install Bip44
```

To install and initiate Ganache:

- Installation: follow the instructions on the Ganache download page https://trufflesuite.com/ganache/ to download and install this tool on your local machine.
- Create a Workspace: when you open Ganache, you are presented with two options for creating a workspace: Quickstart Ethereum and New Workspace Ethereum. Click Quickstart Ethereum:
  ![Ganache](Images/Ganache.png)

---

## Usage

> Application summary<br/>

- View ETH address and available ETH balance:<br/>
  Before making a payment, the users can view an ETH balance available on their ETH address, from which the payment will be made.<br/>

- Select a person to make a payment to:<br/>

  An overview of the employees is provided on the main page and a functionality to choose an individual, to whom the ETH will be transfered, is provided on the sidebar of the application. Once the employee is selected, the user can insert an amount of hours corresponding to the time of service provided by the selected employee. The amount of transfer to be made is calculated based on the hourly wages of the employee and the hours of service and is displayed under the _Total Wages in Ether_<br/>

- Sending a transaction:<br/>
  Once all the information above becomes available, the user can send the transaction. The validated transaction hash will be presented once the payment is made:<br/>
  ![screen](Images/screen.JPG)<br/>

- Viewing the transaction on the Ganache interface:<br/>
  When in Ganache, the user can:<br/>

  1. Check the remainng balance on their address:<br/>
     ![balance](Images/balance.JPG)<br/>
  2. View the block in which the transaction is included - the address of the user and the selected employee, as well as the transfered amount in wei can be verified::<br/>
     ![block](Images/block.JPG)<br/>

  3. Similar information will be visible on the transaction itself:<br/>
     ![tr1](Images/transaction.JPG)<br/>
  4. Finally, when selecting the employee's address on the Transaction above, the adress' balance can be seen too:<br/>
     ![tr2](Images/transaction_2.JPG)<br/>

View the interface and an example of the process of sending ETH:<br/>
![](Images/screen.gif)

> Getting started<br/>

- To use Cryptocurrency Payments Solution first clone the repository to your PC.<br/>
- Use `streamlit run fintech_finder.py` as per the instructions in the [Installation Guide](#installation-guide) to run the application.<br/>

---

## Contributors

Contact Details:

Boris Dudkin:

- [Email](boris.dudkin@gmail.com)
- [LinkedIn](www.linkedin.com/in/Boris-Dudkin)

---

## License

MIT

---
