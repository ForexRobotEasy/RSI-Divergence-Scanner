# RSI Divergence Scanner ReadMe

## About
This ReadMe file provides a detailed description of the code for the RSI Divergence Scanner, developed by Forex Robot Easy Team. Please note that Forex Robot Easy is not the official developer of this product. We are only showcasing a sample code that can work as described in the official product. To find the official developer of this product, please visit MQL5.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy - RSI Divergence Scanner Review](https://forexroboteasy.com/forex-robot-review/rsi-divergence-scanner-last-3-for-30-review/).

## Code Description
The RSI Divergence Scanner is an indicator that detects and alerts the user about divergence patterns in the Relative Strength Index (RSI) indicator. Divergence occurs when the price of an asset and its RSI indicator move in opposite directions, signaling a potential trend reversal.

The code is written in MQL5, a programming language specifically designed for algorithmic trading in the MetaTrader 5 platform. The code consists of several functions, as explained below:

### Input Parameters
- `enableAlerts`: Set to `true` to enable alerts, or `false` to disable alerts.
- `enableSoundAlert`: Set to `true` to enable sound alerts, or `false` to disable sound alerts.
- `enableVisualAlert`: Set to `true` to enable visual alerts, or `false` to disable visual alerts.
- `sensitivity`: The sensitivity parameter for RSI calculations.
- `overboughtLevel`: The overbought level for the RSI indicator.
- `oversoldLevel`: The oversold level for the RSI indicator.

### Global Variables
- `previousDivergence`: A boolean variable that stores the previous divergence flag.

### Initialization
The `OnInit()` function is called during indicator initialization. It adds the indicator buffers and sets the indicator style. Additionally, if alerts are enabled, it adds an alert for RSI divergence detection.

### Indicator Calculation
The `OnStart()` function is called for each new tick in the market. It calculates the current RSI value using the `iRSI()` function. It then checks for RSI divergence using the `checkDivergence()` function. If divergence is detected, it sends alerts based on the user-defined settings. Finally, it updates the `previousDivergence` flag.

### Divergence Checking
The `checkDivergence()` function is used to check for RSI divergence. It calculates the current and previous prices and RSIs. If a bullish or bearish divergence is detected, the function returns `true`, otherwise it returns `false`.

## Product Description
The RSI Divergence Scanner is a powerful tool for traders who use the RSI indicator to identify potential trend reversals. It automatically scans the market for RSI divergences and provides alerts to the user. By detecting these divergences, traders can anticipate possible trend reversals and make informed trading decisions.

Key Features:
- Easy to use: The RSI Divergence Scanner is user-friendly and can be easily integrated into any MetaTrader 5 platform.
- Customizable alerts: Users can enable or disable alerts, sound alerts, and visual alerts according to their preferences.
- Accurate divergence detection: The scanner accurately detects both bullish and bearish divergences, providing reliable trading signals.
- Adjustable sensitivity: Traders can adjust the sensitivity parameter to fine-tune the scanner's performance based on their trading strategies.
- Compatible with multiple markets: The RSI Divergence Scanner can be used on various financial markets, including stocks, forex, commodities, and more.

Disclaimer: Please note that Forex Robot Easy is not the official developer of this product. We only provide a sample code that demonstrates how this product can work. To find the official developer of this product, please visit MQL5.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy - RSI Divergence Scanner Review](https://forexroboteasy.com/forex-robot-review/rsi-divergence-scanner-last-3-for-30-review/).
