
# DeribitX 🚀


## Overview
DeribitX is a low-latency order execution and management system designed for cryptocurrency trading on Deribit Test.
It provides real-time market data streaming, order placement, and risk management using WebSocket connectivity.

## Features
- ✅ **Order Management**: Place, cancel, and modify orders
- ✅ **Market Data Streaming**: WebSocket client for real-time order book updates
- ✅ **Position Tracking**: View open positions and trade history
- ✅ **Low-Latency Execution**: Optimized for fast order placement
- ✅ **Supports Multiple Instruments**: Spot, Futures, and Options

## Installation
### 1️⃣ Prerequisites
- C++17 or later
- CMake
- OpenSSL (for WebSocket authentication)
- WebSocket++ or Boost.Beast (for WebSocket client)

### 2️⃣ Build Instructions
```sh
git clone https://github.com/yourusername/QuantX-Trader.git
cd QuantX-Trader
mkdir build && cd build
cmake ..
make
```

## Configuration
Before running the system, generate API keys from [Deribit Test](https://test.deribit.com/) and set them in `config.json`:
```json
{
  "api_key": "your_api_key",
  "api_secret": "your_api_secret"
}
```

## Running the Trading System
```sh
./DeribitX
```

## Usage
### Order Management
```cpp
TradingClient client;
client.place_order("BTC-PERPETUAL", "buy", 1, 50000);
client.cancel_order("order_id");
client.modify_order("order_id", 50500);
```

### WebSocket Market Data
```cpp
MarketDataStream stream;
stream.subscribe("BTC-PERPETUAL");
stream.start();
```

## Contributing
Pull requests are welcome! Open an issue for feature requests or bug reports.

## License
This project is private and not intended for redistribution.



  "
