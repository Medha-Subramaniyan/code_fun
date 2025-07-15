1. **Season Leaderboard**  
   - Load a season’s box‐score CSV  
   - Compute and sort by advanced metrics:  
     - **PER**, **Usage Rate**, **TS%**  
   - Display top 10 with `df.nlargest(10, 'TS%')`

2. **Shot Chart Visualization**  
   - Pull shot data (x/y coordinates) for a player  
   - Scatter plot with Matplotlib/Seaborn over a court image  

3. **Time Series Analysis**  
   - Aggregate team win‐loss by month  
   - Plot rolling average win% with `df['W/L'].rolling(5).mean()`

4. **Predictive Modeling (Bonus)**  
   - Kaggle “Game Outcome Prediction”  
   - Features: home‐court, rest days, team ratings  
   - Model with `scikit-learn` (logistic regression)


3. **Python Fundamentals in Context**
Skill	Practice Task
Data Types	Load a CSV of player stats, inspect dtypes: df.dtypes
Control Flow	Count number of games where a player scored ≥ 30 points
Functions	Write def ts_percentage(fg, fga, ft, fta): to compute True Shooting Percentage
Error Handling	Wrap file loading in try/except FileNotFoundError
Comprehensions	Build a list of players with PPG > 20:
---

## 5. Learning Resources

- **NBA API Python Wrapper**: https://github.com/swar/nba_api  
- **Basketball-Reference Tutorials**:  
  - Web scraping with `requests` + `BeautifulSoup`  
  - `pandas.read_html()` usage  
- **Books & Courses**:  
  - “Basketball on Paper” by Dean Oliver (stats theory)  
  - Udemy: “Python for Data Science and Machine Learning”  
- **Communities**:  
  - r/nbascripts, r/sportsanalytics on Reddit  
  - GitHub repos tagged **#basketball-analytics**

---