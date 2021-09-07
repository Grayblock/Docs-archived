
# Technical Summary
## System
We are using liquidity pools to finance clean energy projects in the real world. They act as loans in the real world but to the liquidity pools they generate a yield. The yield is collateralized by real payments made from the electricity generator. So it is energy backed payment. To the user the product looks like a yield farm, for which Project Tokens (specific to the Project/s) are put into Project Pools. Project Pools distribute the funds to the owner's wallets by harvesting their proportional amount based on the number of tokens they have staked. The quantity and frequency of payment will be based on smart meter data fed into the smart contract directly.





![Architecture](/smartcontracts.assets/Architecture.png)

![Architecture](/smartcontracts.assets/Architecture2.png)

For example, the energy project maybe a 1 MW solar facility in Vietnam. This project will pay out $0.75 (USDC) per kWh. The sum of the smart meter data collected and published per hour will be collectable every 6 hours and continue to accumulate if not collected. Over 1 day, if the total generation registered is 750 kWh, then the total payment to the contract (which is harvestable by all those who have the project tokens staked) is 750 kWh * 0.75 = $562.50 (USDC).  You as a user have staked 100 Project Tokens (PT1) and the total stake in the Project Pool is 1000 PT1 tokens, then you may harvest 10% or 56.25 USDC after a 24 hour period prior to the user's last harvest.

No return calculations will be provided for users. Instead generation forecasts, Nameplate capacity of the energy project (ie 1 MW), and Power Purchase Price (PPA) $ per kWh will be provided as pool. Other information will include location and Energy Project Developer. Users must self-educate or investigate for themselves as to what the expected yield might be. USDC available for harvesting is paid out at the rate of the smart meter registered (oracle) to Project Pool. Meaning payment should match hourly generation * PPA price per day for that specific energy project. Users may harvest their payments every 6 hours or after. Smart meter data/generation profiles will be provided on an hourly granularity on a rolling 24-hour period.