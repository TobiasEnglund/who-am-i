# who-am-i
Just some info about myself written in Python, because why not?

```
class AboutMe:
    """
    GitHub readme in Python form because why not?
    """

    def __init__(self):
        self.name = "Tobias Englund"
        self.age = 28
        self.location = "Gothenburg, Sweden"
        self.education = {
            "degree": "Vocational, AI & machine learning",
            "school": "IT-Högskolan",
            "years": (2023, 2024)
        }
        self.experience = [
            {
                "role": "AI engineer trainee",
                "company": "Paliscope",
                "keywords": ["AI & machine learning", "Intelligence analysis", "OSINT", "Law enforcement"],
                "years": (2023, 2024)
            },
            {
                "role": "Support & care assistant",
                "company": "GIL, Gothenburg",
                "years": (2020, 2023)
            }
        ]
        self.skills = {
            "languages": ["Python", "basic C#"],
            "packages": [
                "PyTorch", "TensorFlow", "NumPy", "Pandas",
                "Matplotlib", "Seaborn", "Scikit-learn",
                "SpaCy", "fiftyone"
            ]
        }
        self.projects = [
            "Named Entity Recognition (NER) in text",
            "Sound classification (Mel Spectrogram + CRNN)",
            "Image classification (still learning to see)"
        ]
        self.fun_fact = "I whittle magical wands"

    def __str__(self):
        return f"""
            \U0001F30D Hello world, I'm {self.name} from {self.location}!
            I'm curious, analytical, and passionate about AI and have a drive to learn, build, and improve.

            \U0001F393 Education:
            - {self.education["degree"]} at {self.education["school"]} ({self.education["years"][0]}–{self.education["years"][1]})

            \U0001F4BC Current role:
            - {self.experience[0]["role"]} at {self.experience[0]["company"]}

            \U0001F6E0 Skills:
            - Languages: {", ".join(self.skills["languages"])}
            - Packages: {", ".join(self.skills["packages"])}

            \U0001F680 Projects (internship):
            - {self.projects[0]}
            - {self.projects[1]}
            - {self.projects[2]}
            
        PS: I'm gradually building my personal portfolio, but for now I'm focusing on my capstone project (examensarbete) and growing my hands-on experience.
            Fun fact: {self.fun_fact}
        """

if __name__ == "__main__":
    me = AboutMe()
    print(me)
```
