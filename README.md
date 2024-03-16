# LT HiLo Activator ReadMe

## Overview
The LT HiLo Activator is a custom indicator developed by the Forex Robot Easy Team. It is designed to predict Forex trends efficiently. This ReadMe provides an overview of the code and how it works. Please note that Forex Robot Easy is not the official developer of this product, but we are providing a sample code that can work as described in this product.

For detailed reviews and trading results of this product, please visit the [Forex Robot Easy website](https://forexroboteasy.com/forex-robot-review/lt-hilo-activator-review-predict-forex-trends-efficiently/).

## Indicator Details
- Name: LT HiLo Activator
- Copyright: forexroboteasy.com
- Version: 1.00
- Developer: Forex Robot Easy Team
- Link: forexroboteasy.com

## Input Parameters
- CalculationPeriod: The calculation period for the LT HiLo Activator. Default value is 14.

## Global Variables
- ltHiloActivatorBuffer: Indicator buffer to store calculated values.
- trend: Variable to store the current trend (1 for uptrend, -1 for downtrend).

## Custom Indicator Initialization (OnInit)
- Sets the indicator buffer for ltHiloActivatorBuffer.
- Sets the indicator label as 'LT HiLo Activator'.

## Custom Indicator Calculation (OnCalculate)
- Calculates the LT HiLo Activator for each bar.
- Iterates through each bar and checks if the calculation period is reached.
- Calculates the highest high and lowest low within the calculation period.
- Calculates the LT HiLo Activator as the average of highest high and lowest low.
- Checks for trend change by comparing the close price with the LT HiLo Activator.
- If the trend is uptrend (trend = 1) and the close price is below LT HiLo Activator, sets trend as downtrend (-1) and alerts 'Downtrend started'.
- If the trend is downtrend (trend = -1) and the close price is above LT HiLo Activator, sets trend as uptrend (1) and alerts 'Uptrend started'.
- Returns the total number of rates.

## Disclaimer
Please note that Forex Robot Easy is not the official developer of the LT HiLo Activator indicator. We are only providing a sample code that can work as described in this product. To find the official developer of this product, please use MQL5. For detailed reviews and trading results of this product, please visit the [Forex Robot Easy website](https://forexroboteasy.com/forex-robot-review/lt-hilo-activator-review-predict-forex-trends-efficiently/).
