This is a basic template for the project we will make in the Trading Bot Workshop

UB Financial Technology Club
----------------------------------

Welcome to the Trading Bot Expansion Challenge!

In this challenge, you will expand your basic trading bot by adding new features.

You will have 30 minutes - 1 hour(ish) to complete as many expansions as you can!

Each feature you complete earns you points based on difficulty.
Aim for 10+ points! Bonus points available for creativity and clean code!

You can use any resources! But I would advise against AI for full solutions, still allowed though!

Winner will get a prize and top 3 will get mention on discord

Difficulty - 
Easy (1-2 points)
Medium (4-5 points)
Hard (5+ points)

—-
Python-binance documentation (blocked on UBWifi use your phone!) :(
https://python-binance.readthedocs.io/
—--

🟢 Easy Features (1–2 Points


✅ Profit Estimation (2 pts)
Calculate rough profit after each sell:
profit = (sell price - buy price) * quantity
Print the profit from each trade and keep a running total. This helps visualize the bot's performance.

✅ Trade Logging (2 pts)
Keep a log of each buy and sell. Each time the bot makes a trade, write the symbol, action (buy/sell), price, and timestamp to a .txt or .csv file any kind of logging will do. This helps you track and debug your bot’s decisions.


✅  Count Total Number Of Trades (1 pt)
Track the total number of buys and sells your bot has made and print it at intervals. This gives insight into how active your strategy is.

✅  Random Wait Time (1 pt)
Add a randomized delay (e.g., 1–5 seconds) between each loop cycle. This simulates real-world API request pacing and can help avoid rate-limiting.

✅ Color-coded Terminal Output (2 pts)
Use libraries like colorama to color your console messages:

“pip install colorama”
from colorama import init, Fore, Style
init(autoreset=True)  # This resets color after each print

Example:
print(Style.BRIGHT + Fore.CYAN + "BOT ACTIVE")
print(Fore.GREEN + "BUY: Bought 0.1 BTC at $88,500")
print(Fore.RED + "SELL: Sold 0.1 BTC at $89,100")
print(Fore.YELLOW + f"Price update: BTC is now ${current_price}")

Green for buying

Red for selling

Yellow for price info
You do you!








🟡 Medium Features (3–4 Points)

⚙️ Multiple Symbol Support (3 pts)
Instead of trading only one symbol, allow your bot to loop through a list of symbols (e.g., ['BTC', 'ETH']) and trade based on thresholds for each. Great for diversifying!

⚙️ Basic Moving Average Logic (3 pts)
Track the last 5–10 prices in a list and calculate their average.

If current price > average → consider buying

If current price < average → consider selling

Don’t worry about full-on trend detection — just show you can use the average to make decisions.

⚙️ Console Dashboard with Live Updates (2 pts)
(Do at least 3)
Clear the terminal each cycle and print a clean display:

Current price

In-position status

Trade count

Profit so far
Use os.system('cls' or 'clear') to refresh the screen each time.





🔴 Hard Features (4-5+ points)

⚙️ Add Your Own Strategy (You Choose the Logic) (5 points)
Come up with your own twist:

Only trade during certain times of day

Wait for 3 consecutive price drops before buying

Track volume or percent change

If it’s reasonable and shows effort, it counts!


⚙️ End-of-Session Summary (4 points)
At the end of the bot’s run, print a clean report:

Total number of trades

Total profit/loss

How long the bot ran (use time.time() at start/end)


⚙️  RSI Trading Logic (5 points)
Calculate the RSI for the selected trading symbols.

Determine Buy/Sell signals:

If RSI crosses below 30, the bot will buy (considered oversold).

If RSI crosses above 70, the bot will sell (considered overbought).



🟣Extra Features

Any notable feature outside the list may receive points (+5 points)

If you create a frontend (+10 points) 

If you can make Alvi laugh you get (+1 point)

Remember to try and implement the easier features first, and keep track of what you have done!

Good luck, have fun!



Maximum Number of Points you can earn: 40






UB Financial Technology Club 2024-2025
