# Just_MQL_Framework
![GitHub](https://img.shields.io/github/license/justupcorp/Just_MQL_Framework?color=blue)
![Repository Last Release](https://img.shields.io/github/v/release/justupcorp/Just_MQL_Framework?color=light_green)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/justupcorp/Just_MQL_Framework?label=download%20size)
<br>
A cross-language framework that allows you to code your scripts and EAs only once and use it on both MT4 &amp; MT5. <br>
Inspired in [MQL_Easy](https://github.com/Denn1Ro/MQL_Easy) framework.

# Installation
1. Download/clone the repository into your `MQL4/Include` and `MQL5/Include` folders.
2. At the top of your `#include` instructions on your script, add the following line:
```cpp
#include <Just_MQL_Framework/main.mqh>
```
3. Just enjoy!

## Usage
This framework has the following classes:
- [CAccount](https://github.com/justupcorp/Just_MQL_Framework/wiki/CAccount) - To get all the account information
- [CTextFiles](https://github.com/justupcorp/Just_MQL_Framework/wiki/CTextFile) - To handle text files on a very easy way
- [CLogs](https://github.com/justupcorp/Just_MQL_Framework/wiki/CLogs) - To handle logs files with a predefined format
- [CTicks](https://github.com/justupcorp/Just_MQL_Framework/wiki/CTicks) - To handle the candles values
- [CTerminal](https://github.com/justupcorp/Just_MQL_Framework/wiki/CTerminal) - To control the Metatrader terminal buttons
- [CTrading](https://github.com/justupcorp/Just_MQL_Framework/wiki/CTrading) - To handle and control all the trading activities
- [CIndicators](https://github.com/justupcorp/Just_MQL_Framework/wiki/CIndicators) - To handle indicators in both versiones using the MQL4 structure
- [CError](https://github.com/justupcorp/Just_MQL_Framework/wiki/CError) - To handle MQL and internal framework errors

The wiki is currently being made, please, be patient.

# Contributions & Credits
This framework may include our code and third-party code, all the credits will be listed on the respective document. <br>
If you want to collaborate directly with the project, please, feel free to reach us through the `issues` zone.

## Colaborators List
- [@justupcorp](https://www.github.com/justupcorp)
- [@JoniGG](https://github.com/JoniGG)

# TODO
Extend the framework features with other useful libraries that works in both languages
