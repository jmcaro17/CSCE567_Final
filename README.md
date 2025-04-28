# Final Project Writeup — Jesse Caro

## Proposal Outline

Find any details regarding the proposal, feedback, and updates in the proposal folder.

## Summary and Visualization Access

This project builds a data-driven case for why LeBron James is the GOAT (Greatest of All Time) in NBA history.  
It compares LeBron’s career statistics to other legends, including Michael Jordan, across regular season and playoff performance, using a combination of Tableau dashboards and HTML/CSS structured comparisons.

Key Tableau dashboards visualize:

- **Can Current Players Catch LeBron?** (Scoring Trajectory vs Current Stars)
- **Seasons Needed to Catch LeBron** (Projection Timeline)
- **Career Point Totals** (Historical Scoring Leaders)
- **Career Rebound Totals** (Rebounding Comparison)
- **Top 10 Active Scorers**
- **Top 10 All-Time Scorers**

Custom-built comparison sections in the webpage highlight:

- **Regular Season Rankings: LeBron vs Jordan**
- **Playoff Career Rankings: LeBron vs Jordan**

### How to Access the Visualizations:

- All Tableau dashboards are embedded via Tableau Public using official embed codes inside `index.html`.
- All textual visualizations (career comparisons) are styled directly with HTML/CSS for easy reading.
- Simply open `index.html` locally in a browser, no additional libraries required.

---

## Challenges Encountered and Addressed

Several challenges arose during the project:

- **NBA API Pulling Issues:**  
  Pulling clean career and playoff data from the `nba_api` was difficult due to inconsistent schemas between older and newer players. To fix this, I switched from `playercareerstats` to pulling game logs (`playergamelog`) season-by-season and manually aggregated the totals.
  This didn't work so I shifted focus to compare Jordan and LeBron directly in the playoffs.

- **Maintaining Visual Consistency:**  
  Originally, I attempted black-and-gold custom graphics. However, I pivoted to focus entirely on clean, academic white-background layouts to keep the page polished, readable, and cohesive.

- **Building Cohesive Story Flow:**  
  Rather than throwing multiple stats and graphs together, I built the final flow to move logically:  
  _Current players projections → Career scoring dominance → Regular season and playoff comparisons._

---

## Design Decisions

- **Visualization Tool Choices:**

  - **Tableau** was used for interactive charts (scoring projections, total points, rebound leaders).
  - **HTML/CSS** was used for direct stat comparisons (LeBron vs Jordan).

- **Visualization Styles:**

  - Used clean, simple color schemes (white backgrounds, dark text) to prioritize clarity over flashy design.
  - Avoided unnecessary chart clutter — every dashboard has clearly labeled axes, legends, and titles.

- **Interactivity Decisions:**

  - Tableau dashboards allow for zooming, tooltips, and dynamic data exploration.
  - Static HTML sections prioritize fast comparison reading without interaction needed.

- **Design Options Considered But Not Used:**
  - Initially considered using custom Matplotlib graphics (Python).
  - Initially considered adding flashy hover animations, but instead prioritized simple, professional UX.

---

## Future Work

This project could be extended by:

- **Adding Teammate Context:**  
  Pulling data on which teammates were All-NBA, All-Star, or All-Defense during each season, to contextualize playoff wins without elite teammates. I would be able to create visualization showing LeBron's Playoff Success with less talented help then other players in the
  GOAT conversation.

- **Building Interactive Milestone Trackers:**  
  Embedding a dynamic Tableau or JavaScript milestone timeline showing when LeBron hit 5K, 10K, 30K, 40K points relative to other players.

- **Expanding to Predictive Analytics:**  
  Using simple regression models or ML projections to forecast scoring trajectories for Luka Doncic, Shai Gilgeous-Alexander, and Victor Wembanyama.

- **Advanced Statistics and Expanded Datasets:**  
  Future work could involve integrating more advanced statistical measures beyond basic career totals, such as Playoff Statistics, Player Efficiency Rating (PER), Win Shares (WS), Box Plus/Minus (BPM), and Value Over Replacement Player (VORP).  
  Gaining access to professional subscription-based data platforms like Synergy Sports, Second Spectrum, or Basketball-Reference Premium would allow for deeper analytics.  
  This would make it possible to analyze more nuanced aspects of LeBron's impact, such as efficiency by shot zone, clutch-time performance, playoff win probability added, and defensive matchup effectiveness, across a broader sample of players and seasons.  
  It would strengthen the GOAT case not just based on volume stats, but on advanced performance and situational dominance.

---

# Important Note:

- All visualizations were completed using a combination of **Tableau Public** (for complex interactive charts) and **custom HTML/CSS** (for side-by-side stat comparisons).
- No outside Python libraries, Node.js servers, or additional installations are required to view the final project.

---
