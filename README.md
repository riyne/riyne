class GitHubBio:
    def __init__(kevin):
        kevin.name = "Kevin Puthanangadi"
        kevin.location = "Vancouver, BC"
        kevin.internship_experience = [
            {
                "company":  "EPSON",
                "position": "Software Development Intern",
                "duration": "Summer 2023"
            },
            {
                "company":  "ROBOKIDS",
                "position": "Software Engineering Intern",
                "duration": "Summer 2022"
            }
        ]
        kevin.education = [
            {
                "university": "The University of British Columbia",
                "major":      "Electrical and Computer Engineering",
                "graduation": "May 2025"
            }
        ]
        kevin.fields_of_interests = [
            "Software Development",
            "Machine Learning",
            "Automonus Vehicles",
            "Space Exploration",
            "Game Development"
        ]
        kevin.technical_skills = [
            "Python",
            "MATLAB",
            "C/C++",
            "Java",
            "JavaScript",
            "HTML",
            "CSS",
            "Git"
        ]
        kevin.currently_learning = ["Tensorflow"]
        kevin.currently_working_on = ["Personal Website"]
        kevin.goals_2023 = ["Create projects and learn at least 5 new technologies."]
        kevin.hobbies = ["Hackathons", "Video Games", "Movies", "Stocks/Trading"]
        
    def display_bio(kevin):
        bio_dict = kevin.__dict__
        for key, value in bio_dict.items():
            if isinstance(value, list):
                print(key + ":")
                [print(f"- {item}") for item in value]
            elif isinstance(value, dict):
                print(key + ":")
                [print(f"- {k}: {v}") for k, v in value.items()]
            else:
                print(f"{key}: {value}")

if __name__ == '__main__':
    GitHubBio_instance = GitHubBio()
    GitHubBio_instance.display_bio()
