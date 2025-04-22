# Relative Strength Rating Indicator for Daily Timeframe (RS Rating)

This is a TradingView Pine Script implementation for calculating and displaying the Relative Strength (RS) Rating of a stock relative to the S&P 500 index (SPX). It also visualizes the RS line on the chart and provides various options for customizing its appearance and behavior.

## Features

- **Relative Strength (RS) Calculation:** The script calculates a stock's relative strength against the S&P 500 index, with an optional display of a line chart representing the RS.
- **RS New Highs and Lows:** The script allows for the identification and display of new RS highs and lows.
- **Customizable Moving Averages (MA):** You can overlay one or two MAs (SMA/EMA) on the RS line to help identify trends.
- **RS Rating:** The script calculates an RS Rating based on the relative performance of the stock over the past 1, 2, 3, and 4 quarters and assigns a percentile ranking (from 1 to 99).
- **Replay Mode:** It includes an approximate method for replay mode to simulate the RS Rating using constant values.

## Installation

1. **Create a new Pine Script** in TradingView.
2. **Copy and paste** the script code into the editor.
3. **Save the script** with a desired name.
4. Apply the script to any chart to visualize the Relative Strength Rating and its components.

## Inputs & Parameters

### RS Line
- **Hide Rating:** Option to hide the RS Line.
- **Rating Only:** Option to display only the RS Rating (no chart overlay).
- **Color:** Change the color of the RS line.
- **Offset:** Adjust the vertical offset for the RS line.
- **Comparative Symbol:** Choose a different symbol for comparison (e.g., SP:SPX for S&P 500).
- **Plot RS New Highs and Lows:** Option to plot new RS highs and lows.
- **RS New Highs and Lows Types:** You can choose between different types of RS New Highs and Lows (e.g., Historical, RS New Highs Before Price).
  
### Moving Averages (MA)
- **Display MA on RS Line:** Option to display the first and second MAs on the RS line.
- **MA Lengths:** Input the lengths for the first and second moving averages.
- **MA Types:** Choose between Simple Moving Average (SMA) or Exponential Moving Average (EMA).
- **Fill Area:** Option to color the area between the RS line and the moving average.

### Replay Mode
- **Use Fixed Values:** Option to use fixed values for replay mode to simulate RS Ratings in non-updated data environments.

## Usage

Once the script is applied to a chart:

- **RS Line:** The script will display the relative strength line calculated by comparing the price of the stock to the S&P 500.
- **RS Rating:** The script calculates the RS Rating, assigning a percentile score based on performance over different timeframes (1Q, 2Q, 3Q, 4Q).
- **RS New Highs/Lows:** New RS highs and lows will be plotted on the chart as dots, with custom colors for new highs and lows.
- **Moving Averages:** If enabled, two moving averages will be plotted on the RS line to help with trend analysis.

## Customization

You can adjust the following parameters to customize the behavior of the script:

1. **RS Line Settings:** Adjust color, offset, and whether the RS line should be shown.
2. **MA Settings:** Choose the type of MA (SMA/EMA) and adjust the lengths for both the first and second moving averages.
3. **New High/Low Settings:** Enable and customize the appearance of new RS highs and lows.
4. **Replay Mode:** Use fixed values for historical simulation during replay mode.

## Example

Here is an example of what the RS Rating will look like on the chart:

1. The RS line will be plotted against the price chart.
2. Moving averages (if enabled) will be displayed on the RS line.
3. The RS Rating will be calculated and updated based on the performance of the stock relative to the S&P 500.
4. RS new highs and lows will be displayed as blue and red dots respectively, indicating significant changes in relative strength.

## Acknowledgments

This script is based on the work of [Skyte](https://github.com/Skyte) and has been modified for improved performance and additional features. The relative strength calculation is inspired by the [rs-log](https://github.com/Fred6725/rs-log) repository.
