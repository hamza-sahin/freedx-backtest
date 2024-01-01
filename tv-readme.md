█ Our strategy template empowers TradingView users to effortlessly backtest any indicator, enhancing their trading strategy's effectiveness. In addition, users can create automated alerts for seemless connection to Exchanges. This document details our template's features and how to utilize them effectively.

█ [b] Trading Date Settings [/b]

The Trading Date Settings feature in our TradingView script allows you to refine their backtesting parameters by specifying trading dates and hours. This feature enhances the accuracy of the backtest by aligning it with specific time frames and days, ensuring that the strategy is tested under relevant market conditions.

[image]https://www.tradingview.com/x/OhCWvCXB/[/image]

[b]Features:[/b]

⚙️ [b]Enable Trading Between Specific Dates:[/b]
  🎯 Purpose: 
    → Allows you to limit the backtesting of their strategy to a specific date range.
  💡 How to Use:
    → Input the Start Date and End Date for the backtest period.
    → The script will execute the strategy only within this specified date range.

⚙️ [b]Enable Trading Between Specific Hours:[/b]
  🎯 Purpose: 
    → Allows you to limit the backtesting of their strategy to a specific hour range.
  💡 How to Use:
    → Input the start and end hour for in Trading Session section.
    → The script will execute the strategy only within this specified hour range.

⚙️ [b]Enable Trading on Specified Days of the Week:[/b]
  🎯 Purpose: 
    → Gives you the option to conduct backtesting on selected days of the week, tailoring the strategy to particular market behaviours that may occur on these days.
  💡 How to Use:
    → Select the days of the week for the backtest.
    → The script will activate the trading strategy only on these chosen days.

█ [b]Buy/Sell Trigger Settings[/b]

The Buy/Sell Trigger Settings feature is designed to provide users with flexibility in defining the conditions for 'LONG' and 'SHORT' signals based on various indicator types. This customization is crucial for tailoring strategies to different trading styles and market conditions.

[image]https://www.tradingview.com/x/QKZgdOh4/[/image]

[b]Features:[/b]

⚙️ [b]Single-Line Plotted Indicators[/b]:
  🎯 Purpose: 
    → Enables you to select a single-line plotted indicator as a source for backtesting. You can define specific levels to trigger 'LONG' or 'SHORT' signals.
  💡 How to Use:
    → Choose a Single-Line Plotted indicator as the source.
    → Set the top and bottom levels for the indicator.
    → The script triggers 'LONG' signals at the bottom level and 'SHORT' signals at the top level.

[image]https://www.tradingview.com/x/RmCZ9I25/[/image]

⚙️ [b]Two-Line Plotted Indicators[/b]:
  🎯 Purpose: 
    → Allows backtesting with two-line cross plot sources. Signals are generated based on the crossover of these lines.
  💡 How to Use:
    → Select two lines as 'Source 1' and 'Source 2' for the indicator.
    → The script triggers a 'LONG' signal when 'Source 1' crosses above 'Source 2'.
    → Conversely, a 'SHORT' signal is triggered when 'Source 2' crosses above 'Source 1'.

[image]https://www.tradingview.com/x/Rki3KtIP/[/image]

⚙️ [b]Custom Signals[/b]:
  🎯 Purpose: 
    → This setting enables users to define their own criteria for LONG, SHORT, and CLOSE signals based on custom indicator outputs.
  💡 How to Use:
    → Select the custom source for your signals.
    → Define the output values that correspond to each signal type (e.g., “1” for 'LONG', “-1” for SHORT, and “0” for CLOSE).
    → The script will trigger signals according to these custom-defined values.

█ [b]TP/SL Settings[/b]

The TP/SL (Take Profit/Stop Loss) Settings feature is designed to give users control over their profit securing and risk mitigation strategies. This feature allows for setting custom TP and SL levels, which can be critical in managing trades effectively.

[b]Features:[/b]

[b]Custom TP/SL Levels for Long/Short Signals:[/b]
  🎯 Purpose: 
    → Enables users to set specific percentage levels for Take Profit and Stop Loss on long and short signals.
  💡 How to Use:
    → In the TP/SL Settings, input the desired percentage for Take Profit (TP) and Stop Loss (SL).
    → For example, to secure a profit at a 10% price increase on LONG signals, set the “Long TP Percentage” to “10”.

[image]https://www.tradingview.com/x/yKwTRXCY/[/image]

█ [b]Strategy Settings[/b]

Strategy Settings provide a range of options to customize the trading strategy. These settings include leverage, drawdown limits, position direction changes, and more, allowing users to tailor their strategy to their risk tolerance and market view.

[image]https://www.tradingview.com/x/1UdPRfGZ/[/image]

[b]Features:[/b]

⚙️ [b]Enable Leverage[/b]:
  🎯 Purpose: 
    → Allows users to apply leverage to their trades.
  ☢️ Caution: 
    → High leverage can significantly increase the risk of liquidation.
    → High leverage and a high stop-loss price may override your fixed stoploss percentage, adjusting the stop-loss to the liquidation price.
  💡 How to Use: 
    → Set the desired leverage ratio in the Strategy Settings.

⚙️ [b]Enable Drawdown Limit:[/b]
  🎯 Purpose: 
    → Sets a maximum drawdown limit, automatically halting the strategy if this limit is reached, thereby controlling risk.
  💡 How to Use: 
    → Input the maximum drawdown limit (default: 100, min: 0, max: 100).

⚙️ [b]Enable Reverse Position:[/b]
  🎯 Purpose: 
    → Automatically closes a current position and opens a new one in the opposite direction upon detecting a signal for a market trend change.
  🎯 Example: 
    → If a LONG signal is received while in a SHORT position, the script will close the SHORT position and open a LONG position.
  💡 How to Use: 
    → Activate this feature in the Strategy Settings.

⚙️ [b]Enable Spot Mode:[/b]
  🎯 Purpose: 
    → Disables short orders, using short signals only for closing long positions.
  💡 How to Use: 
    → Select the 'Spot Mode' option in the Strategy Settings.

⚙️ [b]Enable Invert Signals:[/b]
  🎯 Purpose: 
    → Inverts all indicator signals, changing LONG signals to SHORT and vice versa.
  💡 How to Use: 
    → Opt for the 'Invert Signals' feature in the Strategy Settings.

⚙️ [b]Enable Trailing Stop:[/b]
  🎯 Purpose: 
    → Triggers a trailing stop order on the exchange instead of a standard stop market order.
  ☢️ Caution: 
    → The backtesting of this feature on TradingView may not accurately reflect actual strategy performance due to discrepancies between TradingView and exchange mechanisms.
  💡 How to Use: 
    → Select 'Trailing Stop' in the Strategy Settings.

█ [b]Advanced Strategy Settings[/b]

Advanced Strategy Settings offer sophisticated methods for managing Stop Loss (SL) and Take Profit (TP) using the Average True Range (ATR). These settings are ideal for traders who want to incorporate volatility into their exit strategies.

[image]https://www.tradingview.com/x/jAGoLzw3/[/image]

[b]Features:[/b]

⚙️ [b]Enable ATR Stop Loss:[/b]
  🎯 Purpose: 
    → Automatically sets the Stop Loss price using the Average True Range at the time of entry.
  💡 How to Use: 
    → Activate 'ATR Stop Loss' to have the SL price calculated based on the current ATR.

⚙️ [b]Enable ATR Take Profit:[/b]
  🎯 Purpose: 
    → Sets the Take Profit price based on the Average True Range at the time of entry.
  💡 How to Use: 
    → Choose 'ATR Take Profit' for TP price determination using ATR.

⚙️ [b]Enable ATR Trailing Stop:[/b]
  🎯 Purpose: 
    → Dynamically updates the Stop Loss price with each new bar, according to the Average True Range.
  💡 How to Use:
    → Activate 'ATR Trailing Stop'.
    → Set the ATR Period to define the number of bars for ATR calculation.
    → Adjust the ATR SL Multiplier to determine the stop loss distance.
    → Modify the ATR TP Multiplier for setting the take profit distance.

█ [b]Trend Filtering Settings[/b]

Trend Filtering Settings are designed to align trading strategies with the prevailing market trend, enhancing the precision of trade entries and exits. These settings utilize moving averages for trend analysis and decision-making.

[image]https://www.tradingview.com/x/jEZ23wOo/[/image]

[b]Features:[/b]

⚙️ [b]Enable Trend Filtering:[/b]
  🎯 Purpose: 
    → Limits trades based on moving average trends, blocking short trades in an uptrend and vice versa.
  💡 How to Use:
    → Enable 'Trend Filtering'.
    → Set Fast and Slow MA Lengths for trend analysis.
    → Select the Timeframe for moving averages.
    → Choose the Moving Average Type for trend filtering.
  🎯 Note:
    → Be cautious with timeframe selections; lower timeframes than the base may cause inconsistencies.

⚙️ [b]Enable Exit on Trend Reversal:[/b]
  🎯 Purpose: 
    → Automatically closes a position when a market trend reversal is detected.
  💡 How to Use: 
    → Turn on 'Exit on Trend Reversal' in the settings.

⚙️ [b]Enable Trend Drawing On Chart:[/b]
  🎯 Purpose: 
    → Visually represents the trend filter directly on the chart for easy reference.
  💡 How to Use: 
    → Activate 'Trend Drawing On Chart' to see the trend filter overlaid on the trading chart.

█ [b]Automated Alert Settings[/b]

Automated Alert Settings are designed to integrate your TradingView script with external platforms like freedx.ai. These settings allow for enhanced strategy execution and management.

[b]Features:[/b]

[b]Enable FreedX Connection:[/b]
  🎯 Purpose:
    →  Establishes a connection between the TradingView script and the freedx.ai platform.
  💡 How to Use:
    → Enable 'FreedX Connection' in the settings.
    → Enter your FreedX Strategy ID to link your specific strategy.
    → Optionally, activate 'Override Allocation Percentage' to bypass the preset allocation percentage in FreedX.
  ☢️ Caution:
    →  Overriding the allocation percentage may result in trade entry errors due to misalignment between entry cost and available balance.

[image]https://www.tradingview.com/x/ksDPCoCn/[/image]

█ [b]Debugging Settings[/b]

Debugging Settings are crucial for users who want to analyze and optimize their strategies. These settings provide tools for visualizing alerts on charts and accessing detailed data outputs.

[image]https://www.tradingview.com/x/2CTazXeN/[/image]

[b]Features:[/b]

⚙️ [b]Enable Alert Plotting:[/b]
  🎯 Purpose:
    → Allows users to visualize trading alerts directly on the chart, aiding in strategy analysis and refinement.
  💡 How to Use:
    → Activate 'Alert Plotting' to draw alerts on the chart.
  ☢️ Caution:
    → It is recommended to disable this feature when creating actual trading alerts, as it can cause latency in signal processing.

⚙️ [b]Enable Debugger Mode:[/b]
  🎯 Purpose:
    → Facilitates strategy debugging by providing detailed data output in the TradingView Data Window.
  💡 How to Use:
    → Turn on 'Debugger Mode' to access real-time data and metrics relevant to your strategy.

█ [b]Additional Settings[/b]

[image]https://www.tradingview.com/x/m83En9VN/[/image]

⚙️ [b]Enable Bar Magnifier[/b]
⚙️ [b]Enable Using standard OHLC[/b]