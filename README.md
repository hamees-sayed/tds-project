# TDS Project



## 1. Exlanation of how I scraped the data

- **Generate `users.txt`**:
   - Queried the GitHub API to find users in Chicago with more than 100 followers.
   - Saved profile links of qualifying users in `users.txt`, one link per line.

- **Create `users.csv`**:
   - For each user in `users.txt`, fetched detailed profile data.
   - Cleaned and standardized fields (e.g., formatted `company` names) and saved to `users.csv` with columns: `login`, `name`, `company`, `location`, `email`, `hireable`, `bio`, `public_repos`, `followers`, `following`, and `created_at`.

- **Generate `repositories.csv`**:
   - For each user in `users.csv`, fetched up to 500 of their most recently pushed repositories.
   - Stored repository details (e.g., `full_name`, `created_at`, `stargazers_count`, `language`, `license_name`) in `repositories.csv`.

## 2. The most interesting and surprising fact I found after analyzing the data  
The most surprising fact I found after analyzing the data was that 85% of the total users had wiki.

## 3. An actionable recommendation for developers based on my analysis
Based on my analysis, actionable recommendations are as follows:
1. Maintain more public repositories. Successful developers average 110 public repositories, compared to 90 for others.
2. Focus on high-impact languages. Top languages among successful developers are: JavaScript, Python, Ruby, Shell, HTML
