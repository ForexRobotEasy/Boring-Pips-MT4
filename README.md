# Boring Pips MT4 Expert Advisor

This is the code for the Boring Pips MT4 Expert Advisor, developed by the Forex Robot Easy Team. This Expert Advisor is designed to trade in a range-bound market by placing buy and sell orders based on the current bid and ask prices.

## Input Parameters

- **LotSize**: The lot size for trading. Default value is 0.01.
- **StopLoss**: The stop loss in pips. Default value is 50.
- **TakeProfit**: The take profit in pips. Default value is 100.
- **MaxSpread**: The maximum allowed spread in pips. Default value is 3.

## Expert Initialization Function

The `OnInit` function is called during the initialization of the Expert Advisor. It sets the maximum allowed spread based on the input parameters.

## Expert Deinitialization Function

The `OnDeinit` function is called when the Expert Advisor is being deinitialized. It does not perform any specific actions in this code.

## Expert Start Function

The `OnTick` function is the main function of the Expert Advisor and is called on every tick. It checks if there is an open position and places buy or sell orders based on the current bid and ask prices.

If there is no open position, it checks if the current bid is below the previous bid and places a buy order. If the current ask is above the previous ask, it places a sell order.

If there is an open position, it checks if the stop loss or take profit level is reached and closes the order accordingly.

## Expert Custom Functions

The `OnTester` function is called when the Expert Advisor is running in the strategy tester. It can be used to perform optimization on historical data.

The `OnLiveTrading` function is called during live trading. It can be used to monitor the performance of the Expert Advisor.

## Product Description

The Boring Pips MT4 Expert Advisor is a range-bound trading system that aims to profit from the price movement within a specific range. It uses a simple strategy based on the current bid and ask prices to determine when to enter and exit trades.

The Expert Advisor places buy orders when the current bid is below the previous bid and sell orders when the current ask is above the previous ask. It also includes a stop loss and take profit level to manage the risk and reward of each trade.

To use this Expert Advisor, simply attach it to a chart in MetaTrader 4 and adjust the input parameters according to your preferences. It is recommended to test the Expert Advisor on a demo account before using it for live trading.

Please note that ForexRobotEasy is not the official developer of this product. We only provide a sample code that demonstrates how this Expert Advisor works. To find the official developer and learn more about this product, please visit the official MQL5 website.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy - Boring Pips MT4 Review](https://forexroboteasy.com/forex-robot-review/boring-pips-mt4-review-overcoming-over-fitting-in-forex/).
