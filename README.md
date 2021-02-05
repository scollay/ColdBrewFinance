# ColdBrew
## Caffeinate Your Investments and Personal Finance
### Market quotes and financial data infrastructure made easy

I’ve long been interested in financial markets and modeling. This past year I’ve been exploring Modern Portfolio Theory, which are investment strategies that blend stocks, bonds, metals, currencies, real estate, and even crypto to provide investment diversification and, in theory, steadier, less volatile returns. 

Unfortunately, as my research progressed and I began to test ideas, I quickly realized that I lacked the basic data infrastructure needed to backtest ideas on a broad range of stocks and markets. What I had in place was often incomplete, took way too long to load, and the code suffered from a bloatload of not-so-useful libraries. I was simply disorganized due to the organic and ad-hoc nature of my data explorations, and it was time for a change.

Assembling, transforming, enhancing, managing, and modelling market and financial data with even a nicely configured laptop or PC is challenging on many fronts, most notably dealing with the sheer amount of data available. Looking back over 20 years, there have been more than 23,000 tradable stocks on the US markets. Some have come and gone, but just the daily quotes history (symbol, date, high, low, close, volume, dividends…) will present over 50 million rows of data with 500 million data points when fully enhanced with technical analysis indicators. Add more history, additional markets, and company fundamentals, and the challenges grow without a solid, scaleable process.

So then… ColdBrew Beans is an infrastructure project written in Python and Pandas to collect, optimize, compress, and enhance market data into a form that can be readily and efficiently used for building models, on a laptop or small footprint cloud server. While there is an SQLite option, the project eschews more complicated database infrastructure such as MySQL or PostgreSQL, preferring to keep everything simple and extremely portable.

I’ve also tested many different libraries, and while there are some really powerful tools and methods out there for dealing with large data sets and quantitative analysis, they also came with drawbacks, such as supporting only subsets of Pandas or older versions of Python, so I’ve settled on just a few libraries that “just worked”.

While one might suggest this is a “Big Data” project, really it’s just a “Large Data” project. I’ve dealt with Big Data professionally, processing 10’s of Billions of user data “events” for a single client using very expensive Amazon infrastructure. That type of infrastructure would be overkill for 20 or even 50 years of market history, and yet, if implemented poorly, this Large Data is certainly big enough to make even a well configured laptop or workstation spin into oblivion, max out CPU, memory, and swap space, and cause the fan to sound like a rocket ready for takeoff.

Once implemented, one can begin to focus on the real challenge, which is building models, investing, and making money!
