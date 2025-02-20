A high-performance C++ trading system for automated order execution on Deribit Test.

Overview

DeribitX is a low-latency order execution and management system designed for cryptocurrency trading on Deribit Test.It provides real-time market data streaming, order placement, and risk management using WebSocket connectivity.

Features

✅ Order Management: Place, cancel, and modify orders
✅ Market Data Streaming: WebSocket client for real-time order book updates
✅ Position Tracking: View open positions and trade history
✅ Low-Latency Execution: Optimized for fast order placement
✅ Supports Multiple Instruments: Spot, Futures, and Options

Installation

1️⃣ Prerequisites

C++17 or later

CMake

OpenSSL (for WebSocket authentication)

WebSocket++ or Boost.Beast (for WebSocket client)

2️⃣ Build Instructions
git clone https://github.com/yourusername/QuantX-Trader.git  
cd DeribitX  
mkdir build && cd build  
cmake ..  
make  

Configuration

Before running the system, generate API keys from Deribit Test and set them in config.json:
{  
  "api_key": "your_api_key",  
  "api_secret": "your_api_secret"  
} 
Running the Trading System
./DeribitX

