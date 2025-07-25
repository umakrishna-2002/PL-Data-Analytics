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

UnderPerformance and Overperformance of the players were calcuated using Goals scored to the xG.

- The players should play morethan 15 matches
  
Why We Use Players With More Than 9 Matches?

- A player who played only a few matches may have very volatile or misleading stats for example  A player with just 1 assist in 1 game might look like a genius playmaker, but it's just a one-off event.
- Metrics like xG or xA are per-event estimations. In small samples, randomness can make players appear to massively overperform or underperform, which isn’t reliable.
- Many features like xA_per_90 or Gls_per_90 become exaggerated when minutes played is too low.Filtering players with a minimum number of matches (or 90s) ensures these ratios reflect actual consistent performance.

          Goals-to-xG Ratio = Goals/ xG

- If the player ends with more than certain ratio he is overperformer.
- If the player ends up scoring less goals than the certain ratio he is underperformer.

  For example:
  - ratio > 1.1 → player scored 10% more than expected → Overperformer
  - ratio < 0.9 → player scored 10% less than expected → Underperformer
  

