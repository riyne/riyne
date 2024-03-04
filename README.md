class GitHubBio:
    def __init__(kevin):
        kevin.internship_experience = [
            {
                "company":  "Boeing",
                "position": "Software Engineering Intern",
                "duration": "Winter 2024"
            },
            {
                "company":  "UBC",
                "position": "Machine Learning Research Assitant",
                "duration": "Fall 2023"
            },
            {
                "company":  "EPSON",
                "position": "Software Engineering Intern",
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
            "Autonomous Vehicles",
        ]

if __name__ == '__main__':
    GitHubBio_instance = GitHubBio()
    GitHubBio_instance.display_bio()
