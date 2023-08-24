# Hello, World! 👋 I'm Konstantinos Papachristos

Aspiring Software Developer | Aegean College Student

Welcome to my GitHub repository! I'm thrilled to have you here as we embark on a journey through code, creativity, and continuous learning.

## 🌱 About Me

🎓 I'm a dedicated student at Aegean College, passionately pursuing a future in software development. My fascination with the ever-evolving world of technology drives me to explore new horizons and craft innovative solutions.

💻 My heart beats in sync with lines of code. The art of transforming ideas into functional software is both my craft and my calling. I'm committed to honing my skills and creating impactful projects that contribute positively to the tech landscape.

🌐 Beyond the confines of spoken languages, I'm an avid learner of programming languages. I find joy in mastering different languages, frameworks, and tools. Each day presents an opportunity for me to absorb new knowledge and translate it into practical applications.

## 🚀 What I Bring to the Table

- A burning passion for software development and problem-solving.
- A relentless curiosity that fuels my learning journey.
- Strong collaboration skills, allowing me to work effectively in teams.
- A dedication to writing clean, efficient, and maintainable code.
- An enthusiasm for keeping up with the latest industry trends.

## 📚 My Most Used Languages

[![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=KostantinosPapachristos&layout=compact)](https://github.com/KostantinosPapachristos)
import requests

def get_language_percentage(owner, repo):
    url = f"https://api.github.com/repos/{owner}/{repo}/languages"
    response = requests.get(url)
    
    if response.status_code == 200:
        language_data = response.json()
        total_bytes = sum(language_data.values())
        language_percentages = {lang: (bytes / total_bytes) * 100 for lang, bytes in language_data.items()}
        return language_percentages
    else:
        print(f"Error: Unable to fetch data - {response.status_code}")
        return None

owner = "YourGitHubUsername"
repo = "YourRepositoryName"
language_percentages = get_language_percentage(owner, repo)

if language_percentages:
    for lang, percentage in language_percentages.items():
        print(f"{lang}: {percentage:.2f}%")


These statistics reflect the languages I'm frequently working with. Feel free to explore my repositories to see these languages in action!



## 📫 Let's Connect!

I'm always excited to connect with fellow developers, enthusiasts, and tech aficionados. Feel free to reach out:

- 📧 Email: kostass.papachristoss@gmail.com
- 💼 LinkedIn: Konstantinos Papachristos (https://www.linkedin.com/in/konstantinos-papachristos-5905ab254/)
