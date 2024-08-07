```python
from wordcloud import WordCloud
import matplotlib.pyplot as plt

skills = [
    'spreadsheets', 'python', 'r', 'sql', 'msSqlServer', 'bigQuery', 'ibmSpss', 
    'powerBi', 'tableau', 'lookerStudio', 'matplotlib', 'seaborn', 'html', 
    'css', 'javaScript', 'flask', 'vueJs', 'firebase', 'cloudflarePages', 'academicWriting', 
    'criticalReview', 'foreignPolicyAnalysis', 'technicalReporting', 'dataCollection', 
    'webScraping', 'troubleshooting', 'linux', 'git', 'canva',
    'microsoftOffice365', 'googleWorkspace', 'libreOffice',
]

skills_text = ' '.join(skills)

wordcloud = WordCloud(background_color=None, mode='RGBA').generate(skills_text)

plt.imshow(wordcloud, interpolation='bilinear')
plt.axis('off')
plt.show()
```


![png](wordcloud.png)
