# PL-Data-Analytics

The dataset is collected from kaggle: contains Stats of football player from Premier League (2021-2022)

Dataset Description:

- Player : Player's name
- Team : Played club in 2021-2020
- Nation : Player's nation
- Pos : Position
- Age : Player's age
- MP : Matches played
- Starts : Matches started
- Min : Minutes played
- 90s : Minutes played divided by 90
- Gls : Goals scored or allowed
- Ast : Assists
- G-PK : Non Penalty Goals
- PK : Penalty Kicks made
- PKatt : Penalty Kicks attended
- CrdY : Yellow Cards
- CrdR : Red Cards
- Gls : Goals scored per 90 mins
- Ast : Assits per 90 mins
- G+A : Goals and Assists per 90 mins
- G-PK : Goals minus Penalty Kicks made per 90 mins
- G+A-PK: Goals plus Assists minus Penalty Kicks made per 90 mins
- xG : Expected Golas
- npxG : Non-Penalty Expected Goals
- xA : Expected Assits
- npxG+xA : Non-Penalty Expected Goals plus Expected Assists
- xG : Expected Golas per 90 mins
- npxG : Non-Penalty Expected Goals made per 90 mins
- xA : Expected Assits made per 90 mins
- npxG+xA : Non-Penalty Expected Goals plus Expected Assists made per 90 mins

Player Positions Analysis
- Identified all unique player positions in the dataset:
   FW, MF, DF, GK, MF,DF, MF,FW, DF,MF, DF,FW, FW,DF

Team & Position Distribution

- Calculated the total number of players for each of the 20 teams.

- Computed the number of players per position for each team.

Top Performers per Team

- Identified the highest goal scorer and top assist provider for each team.

Top Contributors (G+A)

- Determined the player with the highest overall contribution (Goals + Assists) per team.

Disciplinary Records

- Analyzed the number of yellow and red cards received by each team.

- Explored the distribution of cards per player position across all 20 teams.

Overperformer & Underperformer (Forwards Only)

- Focused on forward players (main goal scorers).

- Calculated overperformance and underperformance based on the number of games played, minutes, goals scored (Gls), and expected goals (xG).

- Assessed players with better shooting efficiency.

Team-wise Performance Ratio

- Extended overperformance/underperformance analysis to all 20 teams to identify how each team’s forwards performed relative to expectations.

 Assists Analysis

- Computed total assists per team.

- Determined which positions contributed the most assists overall and for each individual team.



UnderPerformance and Overperformance of the players were calcuated using Goals scored to the xG.

- The players should play more matches
  
Why We Use Players With More Than 9 Matches?

- A player who played only a few matches may have very volatile or misleading stats for example  A player with just 1 assist in 1 game might look like a genius playmaker, but it's just a one-off event.
- Metrics like xG or xA are per-event estimations. In small samples, randomness can make players appear to massively overperform or underperform, which isn’t reliable.
- Many features like xA_per_90 or Gls_per_90 become exaggerated when minutes played is too low.Filtering players with a minimum number of matches (or 90s) ensures these ratios reflect actual consistent performance.

          Goals-to-xG Ratio = Goals/ xG



  
 
