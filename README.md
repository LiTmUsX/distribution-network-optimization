Distribution Network Optimization

This project focuses on designing a cost-effective and reliable distribution network.

The goal was to decide which plants should be active and how demand should be allocated to them while considering fixed costs, transportation costs, plant capacity and a 2-day delivery constraint.

I built a facility-location and transportation optimization model using Python and PuLP. The model was tested under different scenarios to understand how the network behaves when costs increase or when an important plant becomes unavailable.

The project covered:

• 8 candidate plants
• 25 demand zones
• Plant selection and capacity decisions
• Transportation and freight costs
• 2-day delivery constraint
• Single-plant failure analysis
• Fuel-cost sensitivity analysis

The optimized network gave the following results:

• 6.82% annual cost reduction
• ₹21.38B annual savings
• 6 optimized plants compared with 7 active plants in the baseline
• 18 demand zones served
• 95.81% maximum capacity utilization
• Only 0.0022% additional cost from the 2-day delivery constraint

I also tested individual plant failures to understand which locations were most important to the network.

The two most critical plants were:

PLANT07 → +6.53% cost when unavailable
PLANT04 → +4.71% cost when unavailable

This helped identify not just the cheapest network, but also which plants are important for keeping the network resilient.

The project was developed using Python, PuLP, Excel and Power BI.

The Power BI dashboard contains five pages:

1. Executive Overview

Shows the main cost, savings, capacity and network KPIs.

2. Network & Capacity

Shows the selected plants, demand allocation and capacity utilization.

3. Cost Analysis

Breaks down the network cost and compares the optimized network with the baseline.

4. Resilience & Disruption

Shows the impact of plant failures and sensitivity scenarios.

5. Recommendations & Insights

Summarizes the main findings and highlights the plants that are most important to the network.

The repository contains:

notebooks/
Contains the Python notebooks used for the optimization and analysis.

powerbi/
Contains the final Power BI dashboard.

images/
Contains screenshots of the five Power BI dashboard pages.

The main tools used were:

Python
PuLP
Pandas
NumPy
Excel
Power BI
DAX

The main takeaway from this project was that distribution network design is not only about finding the lowest-cost solution. Capacity, delivery time and plant failures also need to be considered when deciding how the network should be structured.
