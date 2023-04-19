# Informations | Enumeration
Informations enumeration identifiers are used in and `CInfo()->`[GetString()](../modules/main/info-getString.md), `CInfo()->`[GetInteger()](../modules/main/info-getInteger.md), `CInfo()->`[GetDouble()](../modules/main/info-getDouble.md) and `CInfo()->`[GetBoolean()](../modules/main/info-getBoolean.md) methods.

### ENUM_INFO_STRING
| ID                        | Description                                         | Index |
| :------------------------ | :-------------------------------------------------- | :---: |
| `TERMINAL_INFO_LANGUAGE`  | The language of the Metatrader Terminal             |   0   |
| `TERMINAL_INFO_COMPANY`   | The company name of the Metatrader Terminal         |   1   |
| `TERMINAL_INFO_NAME`      | The name of the Metatrader Terminal                 |   2   |
| `TERMINAL_INFO_PATH`      | The path of the Metatrader Terminal                 |   3   |
| `TERMINAL_INFO_PATH_DATA` | The path of the Metatrader Terminal data folder     |   4   |
| `ACCOUNT_INFO_NAME`       | The name of the account                             |   5   |
| `ACCOUNT_INFO_SERVER`     | The server of the account                           |   6   |
| `ACCOUNT_INFO_CURRENCY`   | The currency of the account                         |   7   |
| `ACCOUNT_INFO_COMPANY`    | The company of the account                          |   8   |
| `ACCOUNT_INFO_TYPE`       | The type of the account, from (DEMO, REAL, CONTEST) |   9   |

**Notes:**<br>
1. `ACCOUNT_INFO_TYPE` will return the account type as a string. It can return between `"DEMO"`, `"REAL"` or `"CONTEST"`.<br>

### ENUM_INFO_INTEGER
| ID                              | Description                                    | Index |
| :------------------------------ | :--------------------------------------------- | :---: |
| `TERMINAL_INFO_BUILD`           | The build number of the Metatrader Terminal    |   0   |
| `TERMINAL_INFO_MAX_BARS`        | The maximum number of bars in the chart        |   1   |
| `TERMINAL_INFO_CPU_CORES`       | The number of CPU cores                        |   2   |
| `TERMINAL_INFO_DISK_SPACE`      | The disk space in MB                           |   3   |
| `TERMINAL_INFO_MEMORY_PHYSICAL` | The physical memory in MB                      |   4   |
| `TERMINAL_INFO_MEMORY_TOTAL`    | The total memory allocated to Metatrader in MB |   5   |
| `TERMINAL_INFO_MEMORY_USED`     | The used memory allocated to Metatrader in MB  |   6   |
| `TERMINAL_INFO_MEMORY_FREE`     | The free memory allocated to Metatrader in MB  |   7   |
| `TERMINAL_INFO_DPI`             | The screen DPI of the Metatrader Terminal      |   8   |
| `TERMINAL_INFO_LAST_PING`       | The last ping of the Metatrader Terminal       |   9   |
| `ACCOUNT_INFO_LOGIN`            | The login number of the account                |  10   |
| `ACCOUNT_INFO_LEVERAGE`         | The leverage of the account                    |  11   |
| `ACCOUNT_INFO_LIMIT_ORDERS`     | The maximum of pending orders, 0 - unlimited.  |  12   |

**Notes:**<br>
1. The `ACCOUNT_INFO_LIMITS_ORDERS` will return `0` if the maximum of trading orders is unlimited.<br>

### ENUM_INFO_DOUBLE
| ID                         | Description                    | Index |
| :------------------------- | :----------------------------- | :---: |
| `ACCOUNT_INFO_BALANCE`     | The balance of the account     |   0   |
| `ACCOUNT_INFO_CREDIT`      | The credit of the account      |   1   |
| `ACCOUNT_INFO_PROFIT`      | The profit of the account      |   2   |
| `ACCOUNT_INFO_EQUITY`      | The equity of the account      |   3   |
| `ACCOUNT_INFO_MARGIN`      | The margin of the account      |   4   |
| `ACCOUNT_INFO_MARGIN_FREE` | The free margin of the account |   5   |

### ENUM_INFO_BOOL
| ID                                    | Description                                                          | Index |
| :------------------------------------ | :------------------------------------------------------------------- | :---: |
| `TERMINAL_INFO_SERVER_CONNECTED`      | The connection status of the Metatrader Terminal                     |   0   |
| `TERMINAL_INFO_DLLS_ALLOWED`          | The DLLs status of the Metatrader Terminal                           |   1   |
| `TERMINAL_INFO_TRADE_ALLOWED`         | If all the autotrading options are enabled                           |   2   |
| `TERMINAL_INFO_EMAIL_ALLOWED`         | The email status of the Metatrader Terminal                          |   3   |
| `TERMINAL_INFO_NOTIFICATIONS_ALLOWED` | The notifications status of the Metatrader Terminal                  |   4   |
| `TERMINAL_INFO_FTP_ALLOWED`           | The FTP status of the Metatrader Terminal                            |   5   |
| `EXPERT_INFO_IS_TESTING`              | If the expert is running in the strategy tester                      |   6   |
| `EXPERT_INFO_IN_VISUAL_MODE`          | If the expert is running in visual mode of the strategy tester       |   7   |
| `EXPERT_INFO_IS_OPTIMIZATION`         | If the expert is running in optimization mode of the strategy tester |   8   |

**Notes:**<br>
1. `TERMINAL_INFO_TRADE_ALLOWED` will return `true` if all the autotrading options are enabled. This includes:
   1. Autotrading Button
   2. Allow live trading in the expert properties while loading
   3. Allow automated trading in expert properties in the `settings/tools` tab
   4. The account is allowed to trade.<br>
2. `TERMINAL_INFO_NOTIFICATIONS_ALLOWED` will return `true` if the notifications are enabled in the Metatrader Terminal and the Push notification MQ ID is setup properly.<br>