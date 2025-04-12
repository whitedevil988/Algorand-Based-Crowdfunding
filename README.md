
# 🧾 Algorand-Based Crowdfunding dApp

Welcome to this simple, Algorand-powered crowdfunding platform! This project lets you create and contribute to crowdfunding campaigns on the Algorand blockchain. It's built to help you understand how smart contracts and decentralized funding apps can be implemented using Algorand's tech stack.

---

## 🚀 Getting Started

Here’s a step-by-step guide to get everything running locally.

---

### 1. Extract the Project

If you're starting from a ZIP file, just extract it like usual:
- On Windows: Right-click → “Extract All”
- On macOS/Linux: Use your archive tool or run:
  ```bash
  unzip Algorand-Based-Crowdfunding-main.zip
  ```

---

### 2. Install the Prerequisites

You'll need a few tools installed before jumping in:

- **Python 3.7+**
- **pip** (comes with Python)
- **AlgoKit** (recommended for managing the local blockchain)
- Optionally: **Node.js** (if you're planning to mess with the frontend)

To install Python dependencies:
```bash
pip install -r requirements.txt
```

---

### 3. Set Up AlgoKit

If you don’t have AlgoKit yet, install it by running:

```bash
curl -s https://raw.githubusercontent.com/algorandfoundation/algokit-cli/main/scripts/install.sh | bash
```

Then check everything is working with:
```bash
algokit doctor
```

This makes sure your local Algorand setup is good to go.

---

### 4. Start a Local Algorand Node

You can use **AlgoKit LocalNet** to run a test blockchain:

```bash
algokit localnet start
```

Or, if you prefer Sandbox:

```bash
git clone https://github.com/algorand/sandbox.git
cd sandbox
./sandbox up
```

Either way, you'll have a local blockchain to play with.

---

### 5. Set Up Wallets and Accounts

If the scripts don’t auto-create wallets/accounts, you can do it manually:

```bash
./sandbox goal account new
./sandbox goal account list
./sandbox goal clerk send -a 10000000 -f <FROM-ADDRESS> -t <TO-ADDRESS>
```

Just be sure to fund any new accounts before testing transactions.

---

### 6. Run the dApp

Look for the main script in the project root — it's usually something like `main.py` or `crowdfunding.py`. To run it:

```bash
python3 main.py
```

or

```bash
python3 crowdfunding.py
```

This will initialize the smart contract and get things going!

---

### 7. Frontend (Optional)

If there’s a `frontend/` folder:

```bash
cd frontend
npm install
npm start
```

This should launch the frontend on `http://localhost:3000`.

---

### 8. What You Can Do

Once everything’s running, you can:
- 🔧 Create a new crowdfunding campaign
- 💸 Contribute to existing campaigns
- ✅ Close campaigns and withdraw funds

All on a decentralized blockchain, using Algorand smart contracts under the hood.

---

## 🙌 Credits

This project was built as a learning tool to explore Algorand’s smart contract capabilities and build a hands-on crowdfunding dApp.

---

## 📬 Questions?

Feel free to open an issue or fork the project and experiment!
