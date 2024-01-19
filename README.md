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

INSERT INTO profile.skills (id, skills)  
VALUES
  (1, 'SQL'),
  (2, 'Python'),
  (3, 'Tableau'),
  (4, 'R'),
  (5, 'Excel'),
  (6, 'Power BI');
  
INSERT INTO profile.experience (id, company, title)
VALUES
  (1, 'quantium', 'Data Analyst Intern'),
  (2, 'ID/X Partners', 'Data Scientist Intern');

INSERT INTO profile.education (school, degree, major)
VALUES
  ('Universitas Pembangunan Nasional Veteran Jakarta', 'Undergraduate', 'International Relations')
```
