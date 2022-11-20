# Average Rate Option Valuation


Average Rate options are European-style options where the option payoff involves the arithmetic average of the underlying.


Let   be a process of a foreign currency exchange rate, measured in units of base currency   per one unit of foreign currency  , i.e.  .  Let   be a set of averaging dates and   be a corresponding set of normalized weights. Let also   be a payoff settlement date.  Define the arithmetic average of rates as follows

	 	

The payoff of Average Rate option at the settlement date is given by

	 	

where   is the notional principal in foreign currency, K is the option strike, and   (1 or –1) is the call/put indicator.

Let  = 0 be the valuation date and assume  .  Thus, the underlying prices are known at   for  . In case of uniform weights,   for all i. By arbitragy-free pricing theory, the current value of the contract in base currency can be expressed as 

 				(1)

where  is the risk-free discounting factor in the  -risk-neutral world and   is the expectation operator in the same world.   explicitly depends on the spot exchange rate  .

Assuming that   follows a geometric Brownian motion, in  -risk-neutral world, the underlying rate   follows the equation below

                                                           (2)

where   is the risk free interest rate of the base currency,   is the risk free interest rate of the foreign currency, and  is the volatility of the exchange rate. 

The currency exchange rate can be either in direct quote (e.g. USD/EUR) or indirect quote (e.g. CAD/USD). Pricing and delta calculations of each case are discussed below. 

1.	Direct quote:   

The default payoff currency for direct quote is USD. The notional can be either in EUR or USD.

a.	Notional in EUR:
	
		The payoff of the option at the settlement date is given by

                                                          (3)

and the current value of the contract in base currency can be expressed as 

                                          (4)	

The delta (called Delta/USD) is defined by

                                        (5)

where the perturbation on the spot price   is set to be 0.0001. The dollar value Delta/USD (called USD Delta) is computed as

USD Delta =                                                    (6)

where  .

b.	 Notional in USD:
	
	USD Notional is divided by the strike K to get the payout in USD. Thus, the payoff of the option at the settlement date is given by

 

and the current value of the contract in base currency can be expressed as 

 

Delta/USD and USD Delta are computed in the same way using the equations (5) and (6), and they are the same as for the case of EUR notional. 

2.	Indirect quote:   

The default payoff currency for indirect quote is CAD. The notional can be either in CAD or USD.

a.	Notional in USD

		The payoff of the option at the settlement date is given by

 

Note the call option has the form of put option of direct quote as the rates are quoted in the units of foreign currency per base currency. The current value of the contract in foreign currency can be expressed as 

 

where  . delta is always shown in the base currency. The price of the contract and the perturbation of the spot price in delta calculation is in USD/CAD. Thus, we need to write the payoff in USD as follows

		   

Now, the price   is in USD/CAD and the perturbation of the spot is done as   and   where  . Thus, the Delta/USD is defined by

                                          (7)

Similarly, USD Delta is computed as

USD Delta =                                                (8)

where  .

b.	 Notional in CAD:
	
	CAD notional is divided by the strike K to get the payout in CAD. Thus, the payoff of the option at the settlement date is given by

	 	

the current value of the contract in foreign currency can be expressed as 

 

Delta/USD and USD Delta are computed in the same way as in the equations (7) and (8), and they are the same as for the case of EUR notional. 

The valuation approach is similar to https://finpricing.com/lib/FiZeroBond.html


