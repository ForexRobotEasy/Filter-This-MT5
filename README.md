# Filter This MT5

Filter This MT5 is a MetaTrader 5 Expert Advisor designed to filter news updates and execute buy/sell orders based on the filtered news. This software can be used to automate trading strategies that rely on news events and their impact on the market.

## Global Variables

- `g_lastRefreshTime`: Stores the last time the news source was refreshed.

## Expert Initialization Function

The `OnInit()` function initializes the expert advisor. It sets the initial value of `g_lastRefreshTime` to the current time.

## Expert Deinitialization Function

The `OnDeinit()` function is called when the expert advisor is being removed. It can be used to perform any necessary cleanup before the expert is removed.

## Expert Tick Function

The `OnTick()` function is the main function that is called on each tick of the market. It checks if it's time to refresh the news source and calls the `RefreshNewsSource()` function if necessary. It also checks if filtered news is available and calls the `ExecuteOrders()` function if it is.

## Function to Refresh the News Source

The `RefreshNewsSource()` function is responsible for integrating with Forex Factory's economic calendar and fetching news updates. This function should be implemented to update the news source with the latest news events.

## Function to Check if Filtered News is Available

The `IsFilteredNewsAvailable()` function filters news based on specific currencies or keywords. It should be implemented to determine if there are any filtered news events available for trading. The placeholder code in the current implementation always returns `true`, but it should be replaced with the actual implementation.

## Function to Execute Buy/Sell Orders

The `ExecuteOrders()` function is responsible for executing buy/sell orders based on the filtered news. It should be implemented to execute the appropriate trading actions based on the filtered news events. The function should also set stop-loss and take-profit levels for the orders.

Please note that ForexRobotEasy is not the official developer of this product. We only provide sample code that can work as described in this product. For detailed reviews and trading results of this product, you can visit [this link](https://forexroboteasy.com/forex-robot-review/review-filter-this-mt5-forex-software-for-news-filtering/). To find the official developer of this product, please refer to MQL5.

For more information and support, please visit [Forex Robot Easy](https://forexroboteasy.com).
