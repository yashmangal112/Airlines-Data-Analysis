# <div align="center">Airline Data Analysis</div>

## Problem Statement

<div align="justify"> Our company has been steadfastly delivering exceptional air transportation services to our esteemed clientele for numerous years, steadfast in our commitment to ensuring a secure, opulent, and expedient travel experience for our valued passengers. We maintain and operate a diverse fleet of aircraft, encompassing a wide spectrum from small-scale business jets to medium-sized machines. However, our present circumstances are marked by a series of formidable challenges arising from various factors, including more stringent environmental regulations, elevated flight taxes, escalating interest rates, surging fuel costs, and a constrained labor market that contributes to augmented labor expenditures. These challenges exert significant pressure on the company's financial viability, compelling us to actively explore and implement effective remedies to alleviate this predicament. As part of our strategy to confront this complex situation, our organization plans to conduct a comprehensive <b>analysis of our extensive database</b>, with the aim of identifying potential opportunities to <b>maximize the occupancy rate</b> and thus <b>bolster the average profitability generated per seat</b>.
</div>

## Main Business Challenges

1.  <div align="justify">	<b>Enhanced environmental regulations:</b> The aviation industry is encountering mounting demands to mitigate its environmental impact, prompting the adoption of increasingly rigorous environmental legislation. These regulations not only engender elevated operational expenses but also curtail the scope for expansion.</div>
2.  <div align="justify">	<b>Elevated airfare levies: </b> Governments across the globe are imposing more substantial taxes on air travel to address environmental concerns and generate revenue. This surge in airfare levies has contributed to an overall escalation in the cost of flying, consequently dampening the demand.</div>
3.  <div align="justify">	<b>Constricted labor market resulting in escalated labor expenditures: </b> The aviation sector is grappling with a shortage of proficient workforce, leading to heightened labor costs and an upswing in employee turnover rates.</div>

## Objectives

1.  <div align="justify">	<b>Increase the Occupancy Rate: </b> Our focus lies in implementing measures to raise the occupancy rate. This initiative will directly contribute to amplifying the average profit earned per seat while simultaneously addressing the obstacles at hand.</div>
2.  <div align="justify">	<b>Improve Pricing Strategy: </b> It is imperative to develop a comprehensive pricing strategy that adeptly adapts to market fluctuations and aligns with customer preferences. This strategic approach will facilitate the attraction and retention of valuable customers.</div>
3.  <div align="justify">	<b>Enhance Customer Experience: </b> Our utmost priority is to ensure a seamless customer experience, encompassing all stages from booking to boarding. By enhancing these touchpoints, we aim to foster customer satisfaction and loyalty.

The main goal of this study is to identify opportunities to increase occupancy rate in order to boost the average profit earned per seat.
</div>

## Basic Analysis

<div align="justify"> The basic analysis of the data provides insights into the number of planes with more than 100 seats, how the number of tickets booked and total amount earned changed over time, and the average fare for each aircraft with different fare conditions. These findings will be useful in developing strategies to increase occupancy rates and optimize pricing for each aircraft.
</div>

### How many planes have more than 100 seats?

<div align="center">
  
|   | aircraft_code | num_seats |
|:-:|--------------:|---------:|
| 0 | 319           |    116    |
| 1 | 320           |    140    |
| 2 | 321           |    170    |
| 3 | 733           |    130    |
| 4 | 763           |    222    |
| 5 | 773           |    402    |

</div>

### How the number of tickets booked and total amount earned changed over time?

<div align="center">

</div>

### Average charges for each aircraft with different fare conditions

<div align="center">

</div>

## Analyzing occupancy rate

<div align="justify"> Airlines should conduct a comprehensive analysis of their revenue streams with the aim of optimizing profitability. Key metrics to be considered include the annual overall income and the average revenue per ticket. Such research endeavours facilitate pricing optimization efforts and enable the allocation of additional resources toward routes that generate higher profits.
<div>

### For each aircraft, calculate the total revenue per year and the average revenue per ticket

<div align="center">

|   | aircraft_code | total_revenue | ticket_count | avg_per_ticket |
|:-:|--------------:|-------------:|-------------:|--------------:|
| 0 |      319      |  2706163100  |    52853     |     51201      |
| 1 |      321      |  1638164100  |   107129     |     15291      |
| 2 |      733      |  1426552100  |    86102     |     16568      |
| 3 |      763      |  4371277100  |   124774     |     35033      |
| 4 |      773      |  3431205500  |   144376     |     23765      |
| 5 |      CN1      |   96373800   |    14672     |      6568      |
| 6 |      CR2      |  1982760500  |   150122     |     13207      |
| 7 |      SU9      |  5114484700  |   365698     |     13985      |

</div>

<div align="justify">From the above table it is evident that, the aircraft with highest total revenue is <b>SU9</b> and from the barplot in the previous section we can deduce that the price of business class and economy is the lowest in this aircraft. This can be a contributing factor for increase in revenue as more number of people might opt for this aircraft ticket owing to its comparatively lesser cost.
The aircraft with the least total revenue is <b>CN1</b> , and the possible reason for this may be that it offers only economy class with the cheapest price per ticket and this may be due to poor conditions or less facilities and people may associate it with poor service and lower quality.
</div>

### Calculate the average occupancy per aircraft
<div align="justify">
The average occupancy per aircraft is another critical number to consider. Airlines may measure how successfully they fill their seats and discover chances to boost occupancy rates with this metric. Higher occupancy rates can help airlines increase revenue and profit while decreasing operational expenses associated with empty seats.
</div>

<div align="center">

|   | aircraft_code | booked_seats | num_seats | occupancy_rate |
|:-:|--------------:|-------------:|----------:|---------------:|
| 0 |      319      |   53.583181  |    116    |     0.461924   |
| 1 |      321      |   88.809231  |    170    |     0.522407   |
| 2 |      733      |   80.255462  |    130    |     0.617350   |
| 3 |      763      |  113.937294  |    222    |     0.513231   |
| 4 |      773      |  264.925806  |    402    |     0.659019   |
| 5 |      CN1      |   6.004431   |    12     |     0.500369   |
| 6 |      CR2      |  21.482847   |    50     |     0.429657   |
| 7 |      SU9      |  56.812113   |    97     |     0.585692   |

</div>

### Calculate by how much the total annual turnover could increase by giving all aircraft a 10% higher occupancy rate

<div align="center">

|   | aircraft_code | booked_seats | num_seats | occupancy_rate | Inc occupancy rate | Inc Annual TurnOver |
|:-:|--------------:|-------------:|----------:|---------------:|-------------------:|-------------------:|
| 0 |      319      |  53.58318099 |    116    |   0.461923974  |    0.5081163714    |   2976779410.0     |
| 1 |      321      |  88.80923077 |    170    |   0.522407240  |    0.5746479638    |   1801980510.0     |
| 2 |      733      |  80.25546218 |    130    |   0.617349709  |    0.6790846800    |   1569207310.0000002 |
| 3 |      763      |  113.9372937 |    222    |   0.513231053  |    0.5645541581    |   4808404810.0     |
| 4 |      773      |  264.9258065 |    402    |   0.659019419  |    0.7249213609    |   3774326050.0     |
| 5 |      CN1      |  6.004431315 |    12     |   0.500369276  |    0.5504062038    |   106011180.00000001 |
| 6 |      CR2      |  21.48284690 |    50     |   0.429656938  |    0.4726226318    |   2181036550.0     |
| 7 |      SU9      |  56.81211268 |    97     |   0.585691883  |    0.6442610716    |   5625933169.999999 |

</div>

## Conclusion
<div align="justify">To summarize, a comprehensive examination of revenue-related metrics, including annual total revenue, average revenue per ticket, and average occupancy rate per aircraft, assumes paramount importance for airlines in their pursuit of optimizing profitability. Such analyses enable airlines to identify potential areas for enhancement and adjust pricing strategies in accordance with the insights derived from these performance indicators. Particularly, a higher occupancy rate emerges as a pivotal factor contributing to heightened profitability by maximizing revenue generation while minimizing operational costs associated with unoccupied seats.<br>
Furthermore, it is advisable for the airline to undertake a review of aircraft pricing, as excessively low or high prices can significantly influence customer ticket purchasing behaviour. By carefully considering the facilities offered and the overall condition of the aircraft, the airline should establish a judicious and fair pricing structure.
</div>
