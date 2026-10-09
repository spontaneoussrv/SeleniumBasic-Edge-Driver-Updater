# SeleniumBasic Edge Driver Updater

SeleniumBasic lets Excel VBA control a web browser, but it stops working whenever Microsoft Edge updates and the driver falls out of date. This tool downloads the matching Edge driver and installs it into SeleniumBasic for you.

## Contents

| File | Purpose |
|---|---|
| Selenium edge driver Update.py | Finds your SeleniumBasic folder, downloads the Edge driver that matches your installed Edge, and replaces the old edgedriver.exe |
| UpdateDriver.Bat | Manual option: copies an msedgedriver.exe placed next to it into SeleniumBasic |

## How to use

1. Install SeleniumBasic from its [official releases](https://github.com/florentbr/SeleniumBasic/releases).
2. Install the Python packages: `py -m pip install selenium`
3. Run `Selenium edge driver Update.py` whenever Edge updates or your VBA macro reports a driver version error. It asks for administrator rights because SeleniumBasic lives in Program Files.
4. Reopen Excel and run your macro again.

For the manual option, download the x64 driver from [Microsoft Edge WebDriver](https://developer.microsoft.com/en-us/microsoft-edge/tools/webdriver/), place msedgedriver.exe next to UpdateDriver.Bat and run it as administrator.

## Author

Sourab Kumar Saha, Excel VBA and web automation developer. Available on [Fiverr](https://www.fiverr.com/spontaneoussrv).
