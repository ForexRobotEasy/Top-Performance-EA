# Top Performance EA

This is the code for the Top Performance EA, developed by the Forex Robot Easy Team. For detailed reviews and trading results of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/top-performance-ea-review-minimize-drawdowns-with-customizable-forex-software/) website.

## Indicator Parameters
- IndicatorPeriod: The period used for the custom indicator (default: 14)
- AppliedPrice: The price used for the custom indicator calculation (default: PRICE_CLOSE)

## Currency Pairs
- The EA trades on the following currency pairs: EURUSD, USDJPY, GBPUSD, USDCHF, AUDUSD, USDCAD, NZDUSD, EURJPY, GBPJPY, EURGBP, EURCHF, AUDJPY, CADJPY, NZDJPY, GBPCHF, AUDCAD, AUDCHF, AUDNZD, CADCHF, CHFJPY, EURAUD, EURCAD, EURSEK, and EURTRY.

## Customizable Inputs
- LotSize: The lot size used for each trade (default: 0.1)
- TradeDuration: The duration of each trade in minutes (default: 60)
- StopLoss: The stop loss value in pips (default: 50)
- TakeProfit: The take profit value in pips (default: 100)

## Countertrend Detection
- IsCountertrendEnabled: Enable or disable countertrend detection (default: true)
- CountertrendPeriod: The period used for countertrend detection (default: 10)
- CountertrendThreshold: The threshold value for countertrend detection (default: 0.5)

## Trade Statistics
- totalTrades: The total number of trades executed
- totalProfitableTrades: The total number of profitable trades
- totalProfit: The total profit in account currency

## How It Works
The EA is designed to trade on multiple currency pairs using a custom indicator. On each tick, the EA loops through the currency pairs and checks the value of the custom indicator. If the indicator value is positive, a buy trade is executed. If the indicator value is negative, a sell trade is executed.

Before placing a trade, the EA calculates the stop loss and take profit prices based on the current price and the user-defined stop loss and take profit values. The trade is then sent using the OrderSend function.

If countertrend detection is enabled, the EA checks the RSI indicator for each currency pair. If the RSI value is above the user-defined threshold, the trade is skipped to avoid trading against the countertrend.

The trade statistics are updated after each executed trade. The total number of trades, total number of profitable trades, and total profit are printed in the OnDeinit function.

Please note that ForexRobotEasy is not the official developer of this product. This code is provided as a sample that can work as described in the product. To find the official developer of this product, please refer to MQL5.

For more information and detailed reviews of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/top-performance-ea-review-minimize-drawdowns-with-customizable-forex-software/) website.
