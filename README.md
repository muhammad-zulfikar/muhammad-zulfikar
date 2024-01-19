```sql
SELECT 
  name,
  age,
  role,
  education,
  experience,
  projects,
  skills,
  url  
FROM
  profile.info
  LEFT JOIN profile.education
    ON profile.info.id = profile.education.id
  LEFT JOIN profile.experience
    ON profile.info.id = profile.experience.id
    LEFT JOIN profile.skills
    ON profile.info.id = profile.skills.id
WHERE 
  name = 'Muhammad Zulfikar'
LIMIT 10;
```

```sql
INSERT INTO profile.info (name, age, role, url)
VALUES 
  ('Muhammad Zulfikar', 20, 'Data Analyst', 'https://zul.pages.dev'),

INSERT INTO profile.skills (skills)  
VALUES
  ('SQL'),
  ('Python'),
  ('Tableau'),
  ('R'),
  ('Excel'),
  ('Power BI');
  
INSERT INTO profile.experience (company, title)
VALUES
  ('quantium', 'Data Analyst Intern'),
  ('ID/X Partners', 'Data Scientist Intern');

INSERT INTO profile.education (school, degree, major)
VALUES
  ('Universitas Pembangunan Nasional Veteran Jakarta', 'Undergraduate', 'International Relations')
```

<hr>


```python
website_url = "https://zul.pages.dev"

ask_me_about = [
    "Data Analysis", 
    "Operating System",
    "Web Development",
    "International Relations"
]

technologies = {
    "programming_languages": ["Python", "SQL", "R", "Shell"],
    "databases": ["BigQuery", "MsSQLServer", "MySQl"],
    "data_visualization": ["Tableau", "Excel", "PowerBI", "Matplotlib", "Seaborn"],
    "math_tools": ["NumPy", "Pandas", "SciPy"], 
    "software": ["Microsoft 365", "Google Workspace"],
    "webdev": ["HTML", "CSS", "Javascript", "ReactJS"],
    "operating_systems": ["Windows", "Ubuntu", "Android"],
    "editors": ["VSCode", "Jupyter Notebook", "Google Colab", "GitHub.dev", "ViM", "Notepad"]
}

skills = [
    "Decision making",
    "Problem solving", 
    "Analytical thinking",
    "Time management",
    "Quick learner"
]

interests = [
    "Data",
    "Technology",
    "Coding", 
    "Reading",
    "Music",
    "Tetris"
]
```
