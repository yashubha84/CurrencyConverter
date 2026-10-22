<div align="center">

# 💱 CurrencyConverter

**Fast, Simple & Accurate Currency Conversion**

[Features](#-features) • [Quick Start](#-quick-start) • [Usage](#-usage) • [Configuration](#-configuration) • [Contributing](#-contributing)

![build](https://img.shields.io/badge/build-passing-brightgreen)
![version](https://img.shields.io/badge/version-v1.0.0-blue)
![license](https://img.shields.io/badge/license-MIT-green)
![node](https://img.shields.io/badge/node-20%20LTS-339933)
![PRs](https://img.shields.io/badge/PRs-welcome-orange)

</div>

---

## ✨ Why CurrencyConverter?

**CurrencyConverter** is a lightweight, open-source tool that converts amounts between world currencies using up-to-date exchange rates, with no clutter and no hidden paywalls.

Built to be simple to run and easy to extend, it works as a ready-to-use app and as a small codebase you can learn from or build on.

## 🚀 Features

- 🌍 **150+ currencies** supported, including USD, EUR, INR, GBP, JPY and more
- ⚡ **Live exchange rates** fetched from a rates API
- 🔄 **Instant swap** between "from" and "to" currencies
- 🧮 **Accurate calculations** with proper rounding and formatting
- 💾 **Rate caching** to reduce API calls and speed up conversions
- 📱 **Responsive design** that works on desktop and mobile
- 🛡️ **Input validation** with friendly error messages
- 🧩 **Easy to extend** with a clean, modular structure

## 📦 Quick Start

### Prerequisites

- [Node.js](https://nodejs.org/) 20 LTS or newer
- npm (comes with Node.js)
- A free API key from your exchange rate provider (see [Configuration](#-configuration))

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/currency-converter.git

# 2. Move into the project folder
cd currency-converter

# 3. Install dependencies
npm install

# 4. Set up environment variables
cp .env.example .env

# 5. Start the app
npm start
```

Then open **http://localhost:3000** in your browser.

## 🧑‍💻 Usage

1. Enter the **amount** you want to convert.
2. Choose the **From** currency.
3. Choose the **To** currency.
4. Click **Convert** and the result appears instantly.

### Example

| Amount | From | To  | Result      |
|-------:|:----:|:---:|------------:|
| 100    | USD  | INR | ₹ 8,350.00  |
| 50     | EUR  | GBP | £ 43.10     |
| 1000   | JPY  | USD | $ 6.70      |

> ℹ️ Rates shown above are illustrative. Real results depend on live exchange rates.

## ⚙️ Configuration

Create a `.env` file in the project root:

```env
# Exchange rate API
API_KEY=your_api_key_here
API_BASE_URL=https://api.exchangerate-api.com/v4/latest

# App settings
PORT=3000
CACHE_TTL_MINUTES=60
DEFAULT_FROM=USD
DEFAULT_TO=INR
```

| Variable            | Description                          | Default |
|---------------------|--------------------------------------|---------|
| `API_KEY`           | Your exchange rate API key           | —       |
| `API_BASE_URL`      | Base URL of the rates API            | —       |
| `PORT`              | Port the app runs on                 | `3000`  |
| `CACHE_TTL_MINUTES` | How long fetched rates stay cached   | `60`    |
| `DEFAULT_FROM`      | Default source currency              | `USD`   |
| `DEFAULT_TO`        | Default target currency              | `INR`   |

## 🗂️ Project Structure

```
currency-converter/
├── src/
│   ├── index.js          # App entry point
│   ├── converter.js      # Conversion logic
│   ├── api.js            # Exchange rate API client
│   └── utils.js          # Helpers (formatting, validation)
├── public/
│   ├── index.html        # UI
│   ├── style.css         # Styles
│   └── script.js         # Front-end logic
├── tests/                # Unit tests
├── .env.example          # Sample environment file
├── package.json
└── README.md
```

## 🧪 Testing

```bash
npm test
```

## 🛣️ Roadmap

- [ ] Historical rate charts
- [ ] Favorite currency pairs
- [ ] Dark / light theme toggle
- [ ] Offline mode with last-known rates
- [ ] Multi-currency conversion in one go

## 🤝 Contributing

Contributions are welcome! To get started:

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/amazing-feature`
3. Commit your changes: `git commit -m "Add amazing feature"`
4. Push to the branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

Please make sure your code is tested and follows the existing style.

## 📄 License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for more information.

## 🙏 Acknowledgements

- Exchange rate data provided by your chosen rates API
- Badges by [Shields.io](https://shields.io/)

---

<div align="center">

Made with ❤️ by **<your-name>**

⭐ If you find this project useful, please give it a star!

</div>
