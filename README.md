# 🧠 MinionLab - Auto Solana Wallet & Referral Tool

MinionLab is a Node.js-powered automation toolkit designed to streamline Solana wallet connections and referral registrations — perfect for airdrops, mass onboarding, and testing environments.

> ⚙️ Built with ❤️ by [itsmesatyavir](https://github.com/itsmesatyavir)

---

## ✨ Features

- 🔐 **Auto Wallet Connect** — Log into existing Solana accounts from `accounts.txt`
- 👥 **Auto Referral Creator** — Create new fake accounts using referral codes
- 🌐 **Proxy Support** — Full support for HTTP/SOCKS proxies with rotation
- 📦 **ESM Compatible** — Modern JavaScript module support
- 🧪 **Fake Data Generation** — Uses Faker for email/name generation
- 📋 **Console Logging** — Colorful logs and clear status updates

---

## 📁 File Structure

```
minionlab/
├── main/
│   ├── minionLabConnect.js       # Connect existing wallets
│   ├── minionlabAutoreff.js      # Register new fake accounts with referral
│   ├── proxy.js                  # Proxy manager
├── utils/
│   ├── logger.js                 # Colored logging and readline interface
│   ├── solanaHelper.js           # Wallet generation helper using web3 & tweetnacl
├── accounts.txt                  # Input/output of accounts (email:password)
├── proxy.txt                     # List of proxies (HTTP/SOCKS)
├── result.txt                    # Output for connected wallets
├── index.js                      # Main entry script (user selects function)
├── package.json                  # Project metadata and dependencies
└── README.md                     # You're reading it!
```

---

## 🚀 How to Use

### 1. 📦 Setup 

Make sure Node.js is installed. Then run:

```bash
git clone https://github.com/itsmesatyavir/minionlab.git
cd minionlab
```
```bash
unzip minionlab.zip
```


### 2. ▶️ Run the Script
```bash
npm i
```

```bash
node index.js
```

You'll be prompted to:

- Choose a mode:
  - `1` - Connect existing Solana wallets
  - `2` - Register fake accounts using a referral code
- Enter the number of accounts to process or generate
- Enter your referral code (if using mode `2`)

---

## 🧪 Input Formats

### ✅ accounts.txt

Used to connect existing wallets.

```
email1@example.com:password123
email2@example.com:password456
```

### ✅ proxy.txt

Each line should be a full proxy URL:

```
http://username:password@host:port
socks4://host:port
socks5://host:port
```

If `proxy.txt` is missing or empty, it will use your default IP.

---

## 📤 Output

- ✅ `result.txt` — Saves successfully connected Solana wallets in `email:privateKey` format.
- ✅ `accounts.txt` — Will also store new fake accounts generated using referral codes.

---

## 📄 License

This project is licensed under the [Apache-2.0 License](LICENSE).

---

## 🤝 Credits

- Developed by [itsmesatyavir](https://github.com/itsmesatyavir)
- Telegram Support: [@forestarmy](https://t.me/forestarmy)

---

## ⭐️ Star the Repo

If you find this useful, please consider starring the repo. It helps more people discover the project. 💙
