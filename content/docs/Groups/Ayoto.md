# Week 1 Report

## Team Members

| Team Member           | Telegram ID   | Email Address                      |
|-----------------------|---------------|------------------------------------|
| Mostafa Kira          | @mostafakira  | m.kira@innopolis.university        |
| Fedor Krasilnikov     | @chuffjufjf   | f.krasilnikov@innopolis.university |
| Zeyad Alagamy         | @zeyadAjamy   | z.alagamy@innopolis.university     |
| Pavel Roganin         | @winnerjust   | p.roganin@innopolis.university     |
| Ahmed Soliman         | @XDRdvd       | a.soliman@innopolis.university     |
| Md Motasim Bhuiyan    | @pptx704      | m.bhuiyan@innopolis.university     |
| Mohamed Nguira        | @mohamednguira| m.nguira@innopolis.university      |


### Problem Statement
Our software project addresses the critical problem of efficiently diagnosing diseases and connecting individuals with the right doctors. Traditional healthcare systems often lack accessibility and can be time-consuming, leading to delayed or inaccurate diagnoses. These inefficiencies and challenges within the healthcare domain can cause significant stress, delay treatment, and undermine overall patient well-being

### Solution Description
Our platform revolutionizes the healthcare experience by providing a comprehensive solution to the identified problem. Through an intuitive interface, users can input their symptoms, which initiates a guided question-and-answer process. The system collects relevant information to generate a preliminary diagnosis based on advanced algorithms and medical knowledge. Additionally, the platform recommends doctors who specialize in the relevant field, ensuring that users receive the most appropriate care.

#### Main Features List
* A bot for prelimintary diagnosis for the user
* Doctors Online Booking service for partner diagnostic centers
* Dataset with additional list of doctors
* Patient history tracking

#### Additional Features
* Chat with doctors
* Video call with a doctor
* Notifications for the user related to its disease

### Benefits to Users
1- Accurate and Efficient Diagnosis: Users can receive a preliminary diagnosis quickly, reducing anxiety and enabling them to take proactive steps toward treatment.

2- Personalized Doctor Recommendations: Our platform ensures users are connected with doctors who specialize in their specific condition, enhancing the likelihood of successful treatment outcomes.

3- Time and Cost Savings: By eliminating the need for extensive research and multiple doctor visits, our platform saves users valuable time and reduces healthcare-related expenses.

4- Enhanced Access to Healthcare: Our solution bridges the gap between patients and doctors, particularly in remote areas, by providing access to a broader network of healthcare professionals.

5- Improved Patient Experience: With streamlined processes and personalized recommendations, our platform enhances overall patient satisfaction, leading to better healthcare outcomes.

## Differentiation from Existing Solutions
1- AI-Driven Preliminary Diagnosis: By harnessing the power of artificial intelligence (AI), our platform provides users with a preliminary diagnosis for their symptoms. The utilization of advanced algorithms and machine learning techniques ensures a more accurate and efficient assessment.

2- Personalized Doctor Matching: Building upon the preliminary diagnosis, our platform goes beyond generic doctor directories. We take into account the specific condition identified by the AI analysis and match users with doctors who specialize in the relevant field. This personalized approach enhances the likelihood of successful treatment outcomes and fosters a stronger patient-doctor connection.

3- Comprehensive Solution: Unlike standalone symptom checkers or doctor directories, our platform offers an end-to-end solution. From symptom input to preliminary diagnosis and doctor recommendations, we streamline the entire healthcare journey, saving users valuable time and effort.

## User Impact
By empowering individuals with accurate diagnoses and personalized doctor recommendations, our software project has a profound impact on both users and the broader healthcare industry. Key user benefits include improved health outcomes, reduced healthcare costs, increased convenience and accessibility, and enhanced patient satisfaction. Additionally, by streamlining healthcare processes and leveraging technology, our solution contributes to the advancement of digital healthcare, ultimately driving positive change and improved efficiency within the industry.

## User Testimonials or Use Cases
1- Self-Diagnosis: Users experiencing mild symptoms can utilize the platform to conduct a preliminary self-diagnosis. By inputting their symptoms and engaging in the guided question-and-answer process, they can receive insights and initial information about their condition.

2- Access to Specialized Doctors: Patients with specific medical conditions or rare diseases can benefit from the platform's personalized doctor recommendations. By considering the preliminary diagnosis and the user's location, the platform connects them with doctors who specialize in their specific condition, ensuring they receive the most relevant and appropriate care.


## Lean Startup Questionnaire

### What problem or need does your software project address?
Our software project addresses the problem of inefficient disease diagnosis and the challenge of finding suitable doctors for specific conditions. It aims to streamline the healthcare process by providing users with a preliminary diagnosis based on their symptoms and recommending doctors who specialize in the relevant field. This solves the pain point of delayed or inaccurate diagnoses and the struggle to find appropriate healthcare professionals.

### Who are your target users or customers?
Our target users are individuals who are experiencing symptoms and seeking initial guidance for their potential medical conditions. This includes patients who want to validate their symptoms, those seeking a second opinion, individuals in remote or underserved areas, and anyone looking for quick and personalized doctor recommendations. Additionally, our platform can be useful for healthcare professionals as a supportive tool for preliminary assessments.

### How will you validate and test your assumptions about the project?
We will validate and test our assumptions through user feedback and data analysis. By collecting user feedback and conducting surveys, we can gain insights into the user experience and identify areas for improvement. Additionally, we can leverage data analysis to assess the accuracy of our preliminary diagnoses and doctor recommendations, ensuring that our platform is providing the most relevant and up-to-date information.

### What metrics will you use to measure the success of your project?
We will measure the success of our project based on the following metrics:
* User Satisfaction: We will collect user feedback and conduct surveys to assess user satisfaction and identify areas for improvement.
* Accuracy of Preliminary Diagnoses: We will leverage data analysis to assess the accuracy of our preliminary diagnoses and ensure that our platform is providing the most relevant and up-to-date information.
* Accuracy of Doctor Recommendations: We will leverage data analysis to assess the accuracy of our doctor recommendations and ensure that our platform is providing the most relevant and up-to-date information.
* Number of Users: We will track the number of users to assess the growth of our platform and identify opportunities for expansion.

### How do you plan to iterate and pivot if necessary based on user feedback?
We plan to iterate and pivot based on user feedback by continuously collecting and analyzing user feedback. This will allow us to identify areas for improvement and make iterative changes to our platform. Additionally, we will leverage data analysis to assess the accuracy of our preliminary diagnoses and doctor recommendations, ensuring that our platform is providing the most relevant and up-to-date information.


## Leveraging AI, Open-Source, and Experts
Our team has a strategic plan to leverage the following resources for the development and success of our project:

1- AI (Artificial Intelligence):
    AI is a crucial resource that we will extensively utilize in our project. We will use an AI model for making a preliminary diagnosis based on the user's symptoms. 

2- Open-Source:
    Open-source resources play a significant role in our project's development and success. Our project is based on an open-source AI model that we will leverage for making a preliminary diagnosis based on the user's symptoms. Additionally, we will use open-source tools and libraries for the development of our platform.

## Defining the Vision for Your Project

### Overview
Our project aims to revolutionize the healthcare industry by providing an intelligent and user-friendly platform that enables accurate disease diagnosis and personalized doctor recommendations. By leveraging artificial intelligence (AI) and advanced algorithms, we address the problem of inefficient diagnosis and the challenge of finding suitable doctors for specific conditions. Our platform streamlines the healthcare process, saving time and effort for users while ensuring they receive the most relevant and effective medical care.

### Tech Stack
* Frontend: React.js, TailwindCSS, nextJs
* Backend: Python, Java, LUA
* Database: PostgreSQL
* Mobile: Flutter
* AI: NLP, Decision trees

### Anticipation Future Problems
1- Data Privacy and Security: We anticipate the need for robust security measures to protect user data and comply with privacy regulations. Implementing encryption, secure data storage, and strict access controls will be essential.

2- Integration with External Systems: Ensuring seamless integration with external databases, medical resources, and location-based services may pose technical challenges. We will proactively address compatibility issues and potential API limitations.

3- Scalability and Performance: As the user base grows, handling increased traffic and ensuring real-time response will require careful consideration. We will plan for scalability and performance optimization to maintain a smooth user experience.


# Week 2 Report

## Architecture Design

### Component Breakdown
1. AI Diagnosis Module: Utilizes advanced AI algorithms to analyze symptoms and provide preliminary diagnoses.
2. Doctors Recommendation Engine: Matches users with suitable doctors.
3. User Profile Management: keeps track of user profiles and their medical history.

### Data Management
The platform will employ a relational database management system. We will use PostgreSQL to store user profiles, symptom data, preliminary diagnoses, and doctor information.

### User Interface(UI) Design:
We have agreed on the main design for our website and mobile application. The designs are available on figma and can be accessed through the following links:
* [Landing Page](https://www.figma.com/file/vfig3GqohPdEdZ9T5iobsG/Untitled?type=design&node-id=0%3A1&t=UuhiSCxQt9IUuGUc-1)
* [Mobile Application](https://www.figma.com/file/yuFRxpkTyESOVsHQonAHRg/Untitled?type=design&node-id=0%3A1&t=DSkRwfnDLBPvE8Du-1)


### Integration and APIs
We will be using the following APIs:
* Symptom Checker API
* Auth0 API

### Scalability & Performance
Our platform will utilize Kubernetes (k8s) and Nginx to ensure scalability and optimal performance. Kubernetes allows for easy scaling by dynamically allocating resources based on demand, while Nginx serves as the load balancer, distributing traffic across multiple instances of the application. These technologies work together to handle increased user loads and deliver a high-performance experience.

### Security and Privacy
The platform will incorporate robust security measures to protect user data and ensure privacy. This includes implementing authentication and authorization mechanisms, encrypting sensitive data at rest and in transit, and adhering to relevant security standards and best practices.

### Error Handling and Resilience
We will employ unit tests for comprehensive code validation and utilize Grafana and Prometheus for effective monitoring and alerting. This approach ensures robust error handling, proactive issue identification, and enhances application resilience.

### Deployment and DevOps
We will implement CI/CD (Continuous Integration/Continuous Deployment) using Travis and Jenkins. These tools will automate the build, testing, and deployment process, ensuring efficient software delivery.


## Questionnaire
* We are not utilizing project-based books
* We currently do not have a mentor
* We expanded our understanding for the technical stack mainly by researching and reading articles online
* We do not feel that we are facing knowledge gaps at the moment
* We organized several meeting for for discussion and knowledge sharing
* We utilized AI by using large language models for understanding some technical aspects that were not clear to us

## Tech Stack and Team Allocation
Assignment of team members roles in the project was done according to the experience of each member in the team and the projects he worked on before.

The technical roles in the team is assigned as follow:
Frontend: Zeyad Alagamy
Backend: Fedor Krasilnikov, Md Motasim Bhuiyan, Ahmed Soliman
Mobile Application: Mohamed Nguira, Pavel Roganin

The business side of the project is managed by Mostafa Kira and Md Motasim Bhuiyan. They are working on tasks such as market research & Analysis, contacting potential partners, writing business plan, and communicating with investors

## Challenges
We couldn't find mentors to guide us in developing the project.

## Accomplishments
* We have completed the architecture design for our platform
* We have completed the UI design for our platform
* We created a landing page
* We found a potential investor for our startup
* We communicated with one hospital to partner with us


{{< hint danger >}}
**Feedback**  


**1. Component Breakdown**

Good, but you need to categorise those mention into Frontend/ backend.

**2. Data Management**

Good

**3. UI Design**

I like the design very much. But what the Landing page different design than the mobile app? 
Try to keep consistent design among platforms in order not to confuse users. 

I like the chat design, but it missing the send button. also how will you handle if the user will write a big prompt? 

**4. Integration and APIs**

Missing

**5. Scalability and Performance**
Good

**6. Security and Privacy**
Good

**7. Error handling and Resillience**
Unit testing will help you test the alit of the current code. But this is only one part of handling errors. You need to use a mechanise to handle errors while he program are in production. 
Since you are suing Mobile try to use crashlytics 

**8. Deployment and DevOps**
Good

**Answering questioner**
Answering for the questioner is very short, and doesn’t reflect much consideration. 
You should explain why you don’t have a mentor. 
I hardly believe that you have no gap in your knowledge ( so you are perfect at everything? )

You should redo them.

> We couldn’t find mentors to guide us in developing the project.

The mentor job is not all about the challenges. beside you didn't face any challenge?.
 
please try to be more realistic.

**Overall**
The report is good. But you should really take into consideration the questioner answering properly. If you did it you would have gotten a full mark.

and try to be more realistic.

Grade 4/5


_Feedback by Moofiy_
{{< /hint >}}