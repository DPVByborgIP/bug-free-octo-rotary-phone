https://colab.research.google.com/drive/11WMP0LZ-NTW2aG5p07B7rBO6En9n2LJQ?usp=sharing

For example, if a $100 stock has a history of spiking 10% with each earnings release, 
The earning release events increases the volatility
 
We might have the following scenarios based on the earning event
$90 - current - $110

Writer
Scenario: Stocks drops
	Write a call option: CDD-MM-XXXX108
	The market price at expiration/evaluation stays below Strike price
	The premium is earned

Scenario: Stocks rises
	Write a put option: PDD-MM-XXXX91
	The market price at expiration/evaluation stays above Strike price
	The premium is earned

Buyer
Scenario: Stocks rises
	Buy a call option: CDD-MM-XXXX108
	The market price at expiration/evaluation rises above Strike price
	The profit (Mp-Sk) - P

Scenario: Stocks drops
	Buy a put option: PDD-MM-XXXX108
	The market price at expiration/evaluation drops below Strike price
	The profit (Sk - Mp) - P 

Writer

Scenario: Stock drops:
    * Write a call option: CDD-MM-XXXX108
    * If the market price at expiration/evaluation stays below the strike price ($108 in this case), the writer keeps the premium earned from selling the call option.
    * This strategy is profitable for the writer if the stock price remains below the strike price because the 


Scenario: Stock rises:
    * Write a put option: PDD-MM-XXXX91
    * If the market price at expiration/evaluation stays above the strike price ($91 in this case), the writer keeps the premium earned from selling the put option.
    * This strategy is profitable for the writer if the stock price remains above the strike price because the put option will expire worthless.

Buyer:
Scenario: Stock rises:
    * Buy a call option: CDD-MM-XXXX108
    * If the market price at expiration/evaluation rises above the strike price ($108 in this case), the buyer profits from the difference between the market price and the strike price, minus the premium paid for the option.
    * This strategy is profitable for the buyer if the stock price exceeds the strike price by more than the premium paid for the call option.


Scenario: Stock drops:
    * Buy a put option: PDD-MM-XXXX108
    * If the market price at expiration/evaluation drops below the strike price ($108 in this case), the buyer profits from the difference between the strike price and the market price, minus the premium paid for the option.
    * This strategy is profitable for the buyer if the stock price falls below the strike price by more than the premium paid for the put option.
