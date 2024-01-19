### Hi there 👋

<!--
**muhammad-zulfikar/muhammad-zulfikar** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

```sql
SELECT 
  name,
  age,
  skills,
  education,
  experience,
  projects,
  url  
FROM
  profile.info
  LEFT JOIN profile.education
    ON profile.info_id = profile.education_id
  LEFT JOIN profile.projects
    ON profile.info_id = profile.projects_id
  LEFT JOIN profile.experience
    ON profile.info_id = profile.experience_id 
WHERE 
  name = 'Muhammad Zulfikar'
GROUP BY
  name
LIMIT 10;
```
