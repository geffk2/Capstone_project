---
weight: 1
bookFlatSection: true
title: "ComplianceGuard"
---
# **ComplianceGuard** 

{{< hint danger >}}

ComplianceGuard is a cross-platform application that can check whether an employee is wearing special equipment or not.
{{< /hint >}}

# **Week #1**


| Team Member            | Telegram ID   | Email Address       |
|------------------------|---------------|---------------------|
| Team Member (Lead) 1          | @BikTracker | d.kuzmin@innopolis.university     |
| Team Member 2          | @Mosiramakata | i.belyaev@innopolis.university     |
| Team Member 3          | @isqisq | i.ishkineev@innopolis.university     |
| Team Member 4          | @dudlas | r.sayfeev@innopolis.university     |
| Team Member 5          | @ADari_Ka | d.kalashnikova@innopolis.university     |
| (Optional) Team Member 6 | @FateeeGW | m.gubaidullin@innopolis.university     |
| (Optional) Team Member 7 | @NoNesmer | v.rublev@innopolis.university     |


### **Value Proposition**

We can agree that a builder, a factory worker or an employee of a nuclear power plant are quite dangerous professions. Working, they risk their lives, so to reduce the risk, people have invented special equipment for them. But the problem is that people often neglect precautions, so many workers do their work without special equipment. Such negligence significantly increases the likelihood of an accident, so there must be a way to monitor whether workers are wearing special equipment. Now this is controlled by operators who have to sit next to the cameras all the time and check whether people are wearing special equipment. But this method is unreliable due to the human factor, so we want to create an application that will check whether an employee is wearing special equipment instead of human. How it will work: An artificial intelligence model will receive video from cameras and highlight people in red if they are not wearing equipment, and green otherwise. If the program sees a violation of the rules, it will send a warning message with a screenshot from the camera to the specified location (email, phone message, etc.). Our program will constantly monitor employees, so it will instantly detect violations of safety regulations and report it. By choosing our program, you eliminate the human factor, save your time and money. There  already exists a similar program [**EYECONT**](https://www.mallenom.ru/products/eyecont/kontrol-ispolzovaniya-siz/), but this is just a model of artificial intelligence inside the cameras. Our program is an application, so you can see what is happening on a particular camera, anytime and anywhere. In general, our application can benefit the industry, because by using our program, companies can stop worrying about the safety of their employees.

## **Lean Startup Questionnaire**

1. The problem of compliance with safety regulations by employees
2. Owners of factories, building companies, seaports, ...
3. Interview our target customers, analyze the number of accidents under different conditions
4. Number of wrong predictions made by the model, wholeness of predictions, application user experience(for better design and functionality)
5. Remove or improve features which doesn't work, add features which users want to have


## **Leveraging AI, Open-Source, and Experts**

Explain how your team plans to leverage the following resources for the development and success of your project:

- AI (Artificial Intelligence):
- Open-Source:
- Experts in relevant domains:

AI: our application is build around a CV model
Open-Source: Our ML engeneers can use models from Open-Source to study and improve the model in our program
Experts in relevant domains: Our developers will ask advices from more experienced specialists to improve quality of the application

## **Inviting Other Students**

For now we are not planning to invite other students in our project

## **Defining the Vision for Your Project**

Overview: Our project is designed for managers of companies whose employees must wear special equipment. This is an application that allows you to determine by video whether a person is wearing special equipment or not. If a person is not wearing equipment, he highlights it in red, otherwise - in green. It will allow the manager to receive a notification when workers are at the workplace without special equipment, to view video from cameras in real time.

**Schematic Drawings:** 
![image](/ComplianceGuard/week1capstonediagram.png)

{{< hint danger >}}

**Feedback**  
This chart is more of a platitude than actual description of the project. Consider using more specific charts explaining something 
{{< /hint >}}
#### Tech stack: 
- Design: Figma
- Frontend: Javascript, HTML, CSS, ReactJS
- Backend: Python, FastAPI/aiogttp+async, pydantic
- AI: OpenCV, PyTorch

Anticipating Future Problems: Potential problems are: Big complexity of AI model, time to train the model, limited GPU, unknown dataset(what is dataset itself, how much data in it), pretty complex backend(mainly features like sending messages, connecting to the cameras). How can these problems be solved: Find additional GPU to spend less time on training, improve dataset if necessary(reversing videos, rotating, etc.), ask experienced specialists to help us with problems(with model creation, backend development).

Elaborate Explanations: The most critical component is implementation of AI model. It should predict well, but should not be too complicated(otherwise it wont have time to train well). Frontend is going to be pretty simple, and algorithms for additional functionality on backend side(working with cameras, sending messages) are still going to be learned. About flow of the project development - it will be based on Agile and Scrum, due to the fact that in the end we should present only MVP of the project.

{{< hint danger >}}

**MVP plans**
Above I described the final version of the project. In MVP we will include a cross-platform application, that takes a pre-recorded video and apply a created CV model to it.
{{< /hint >}}

# **Week #2**

**Tech stack**

- Design: Figma
- Frontend: Javascript, HTML, CSS, ReactJS
- Backend: Python, FastAPI/aiogttp+async, pydantic
- AI: OpenCV, PyTorch

{{< hint danger >}}

This seems to be a detailed list of the technologies needed to finish the project. However, it was part of the weekly task to make a personalized allocation of the tasks for the project. 
{{< /hint >}}

**Architecture**

- Component Breakdown: Our project has the following components: Design, Frontend, Backend and CV model. First, design creates a general view of both mobile and computer versions of the application. Then, Frontend makes this design come true and prepares for future requests from backend. Backend works with database(In final version), process metadata taken from frontend, works with message broker and sends messages to specified paths. CV model takes the video and process it.

- Data Management: We decided to use dvc as a management tool for our models. It is very convinient, because using dvc we can keep old models, to return to them if necessary, use external GPU to train models and combine models between each other. To store data we will use cloud storage.

- Scalability and Performance: We are using micro service architecture, because it is much easier to maintain and develop than monolith architecture. After MVP we have a lot of ideas on how to improve our application, many of them are already written above: Add live work with real cameras, find smaller equipement on employees, add authorisation for security.

- Security: For MVP our application does't require any security, but in future, when many people will work with our application, we plan to add authorisation, that can be protected by hard passwords, keys generation or two-factor authentication.

- Error handling: In MVP, there aren't a lot of things that can go wrong. We will have only uploading of a video and work of model on it.
But later, if something go wrong, we will send an error with it's code and description to some address, where we will be able to learn and then fix it. On user's side, when error occur, the video will just stop and pop-up with warning will appear.


**Current progress**

Now we are ending creation of the design, our ML team received a dataset today and actively learn it. We got a cloud from university for our models and agreed with ML lab to get GPU from them. We have daily meetings with our customer that agreed to give us some help with code and ideas if necessary(special person from the company will help us). Also we were added two people from magistracy that will help us with our project, which is a significant boost.

{{< hint danger >}}

This is a good news that your project got support from the client and now you have more master students helping you out. In general, I feel confident that ComplianceGuard team would be able to finish the Capstone with an MVP - you have control and support from the client, students and ML lab. However, the weekly progress report is short and it's hard for me to understand how the team is progressing. No information on the model, tools and approaches. For example, you can add a Figma layout as a result of the work - a screenshot would suffice. Consider adding more details on your progress report and show your progress in a little more expanded manner.
Overall, can be a good job on the project, not so on the report.  
Report - 3/5

{{< /hint >}}