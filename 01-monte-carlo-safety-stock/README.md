Monte Carlo Safety Stock Project — Excel
The problem
A shop sells about 120 bottles of 1L sunflower oil every day, but daily sales keep changing — some days more, some days less. New stock takes 6 days to arrive. How much extra stock should the shop keep so the shelf almost never goes empty — without locking too much money in stock?

What I did

Ran demand 10,000 times in Excel (Monte Carlo simulation) using average daily sales of 120 bottles and daily change of 25 bottles.
Found the safety stock two ways — a formula method and the simulation method — and both agreed.
Compared the total cost (storing cost + stock-out loss) at 6 service levels: 85% to 99.9%.
The answer

Keep 142 bottles as safety stock. Order new stock when the level falls to 862 bottles.
At 99% service level the total cost is the lowest: ₹5,377 for one year — about ₹2,235 cheaper than the common 95% level, with fewer stock-outs.
Trade-off: ₹19,880 (142 × ₹140) stays invested in safety stock.
Tools: Microsoft Excel only — NORM.INV, RAND, PERCENTILE, FREQUENCY, INDEX.

What I learned
More safety stock is not always better. After one point, storing cost grows faster than the stock-out loss it saves. The cheapest point can be found — it does not have to be guessed.

Note: The Excel file is set to manual calculation. Press F9 to run a fresh simulation; results move slightly with each run because demand is random.
