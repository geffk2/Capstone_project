# **LeetForces**

Hi! We a group called "LeetForces" and we do the `LeetForces` project.

# **Weekly reports**

{{< expand "Week 1 report" >}}

## **Team Formation and Project Proposal**


### **Team Members**

| Team Member            | Telegram ID   | Email Address       |
|------------------------|---------------|---------------------|
| Anton Nekhaev          | @anekhaev | a.nekhaev@innopolis.university     |
| Alexander Buchnev      | @pwn0id | a.buchnev@innopolis.university     |
| Vladislav Danshov      | @vladislav_danshov | v.danshov@innopolis.university     |
| Elina Akimchenkova     | @akmchnkv     | e.akimchenkova@innopolis.university     |
| Vladimir Surikov       | @MasterLogick | v.surikov@innopolis.university    |
| Georgiy Sapronov       | @qexik | g.sapronov@innopolis.university     |

### **Value Proposition**

- **Problem**: During the first-year of study at Innopolis University we (as students) faced a problem with the local code submission system called "codetest".
    It had some fatal flaws in its implementation regarding the security aspects, as well as stability, so we decided to give our version of codetest a try.
- **Solution**: As a solution, we propose a microservice architecture system which is oriented for easier scalability, management and security.
    The architecture consists of  several independent microservices.
- **Benefits to Users**: Our system is beneficial to future Innopolis University students and professors in the sense that the proposed system is secure (as far as
    we are informed about existing software flaws), reliable, easy to maintain and use, scalable, and provides neat UX/UI.
- **Differentiation**: The system we develop offers Innopolis University a more secure and convenient way to check and generate assignments for students.
    It ensures security by addressing known software vulnerabilities and offers reliability, easy maintenance and usability, scalability, and a user-friendly interface for a seamless experience.
- **User impact**: Our software project at Innopolis University has a significant impact on users, educational society, and the industry. It improves workflows
    by offering a scalable and secure microservice architecture system for assignment submission and grading. Users are empowered with a reliable and user-friendly interface, allowing them to focus on their tasks with confidence.
- **Use cases**:
    - Assignment Submissions
    - Plagiarism Detection
    - Grading and Evaluation
    - Academic Progress Tracking

## **Lean Startup Questionnaire**
1. **What problem or need does your software project address?**
Our software project addresses the need for a secure and stable code submission system, addressing flaws in the existing
"codetest" system at Innopolis University.

2. **Who are your target users or customers?**
Our target users are the students and professors at Innopolis University who require a reliable and user-friendly
platform for assignment submission, grading, and feedback.

3. **How will you validate and test your assumptions about the project?**
We will validate our assumptions through user interviews and usability testing gathering feedback from students and
professors to analyze their experiences and suggestions.

4. **What metrics will you use to measure the success of your project?**
We will measure success through metrics such as user satisfaction, adoption rate, security incidents, system stability,
assignment turnaround time, and improvements in assignment quality based on professor feedback.

5. **How do you plan to iterate and pivot if necessary based on user feedback?**
We will gather user feedback through direct communication, identifying areas for improvement and prioritizing them for
subsequent iterations. We are open to pivoting our approach based on user feedback, ensuring the system meets the needs
and preferences of our users.

## **Leveraging AI, Open-Source, and Experts**

1. **AI (Artificial Intelligence)**:  We will leverage AI technology to improve the code submission system through
plagiarism detection enhancing efficiency and accuracy for students and professors.

2. **Open-Source**: By utilizing open-source libraries, frameworks, and tools, we can expedite development, reduce
costs, and tap into the collective knowledge and contributions of the open-source community, allowing us to focus on
customization and integration for our specific project needs.

3. **Experts in Relevant Domains**: Our team will ask for help from experts in relevant domains to achieve the best possible
solution.

## **Defining the Vision for Your Project**
1. Summary: Our project addresses the need for a secure and reliable code submission system at Innopolis University. It
    offers a streamlined workflow, improved security, and enhanced user experience, benefiting students and
    professors by simplifying assignment submission and grading processes. The project fosters a culture of excellence
    and innovation within the university community.
2. Schematic drawing:
```
                                   +-----------------+
                                   |                 |
                                   |   Database      |
                                   |  (PostgreSQL)   |
                                   |                 |
                                   +--------+--------+
                                            |
                                            |
                                            |
          +-----------------+      +--------+--------+      +-----------------+
          |                 |      |                 |      |                 |
          |                 |      |                 |      |                 |
          |  Orchestrator   +------+     Backend     +------+    Frontend     |
          |                 |      |                 |      |                 |
          |                 |      |                 |      |                 |
          +--------+--------+      +-----------------+      +-----------------+
                   |
       +-----------+-----------+
       |                       |
+------+-------+       +-------+------+
|              |       |              |
| Test runner  |       | Test         |
|              |       |  generator   |
|              |       |              |
+--------------+       +--------------+
```

As depicted above, the project consists of several modules:
- Frontend - the service which provides interaction with the user
- Backend - the service which handles requests from bot and forwards them according to their destination
- Orchestrator - the service which manages test generation and user submission execution and checking
3. **Tech stack**: Docker, docker-compose, GitHub actions CI/CD, Prometheus, Grafana, postgreSQL, Flutter, Python,
XMLRPC.

4. **Anticipating Future Problems**:
Potential challenges during project development and deployment include technical complexities, resource limitations,
time constraints, and dependencies on external systems. To mitigate these risks, we will plan meticulously, maintain
open communication within the team, leverage scalable cloud services and prioritize essential functionalities.

5. **Elaborate explanations**:
- Our project utilizes a microservice architecture, enabling scalability, management, and security. Independent
    microservices handle user authentication, assignment submission, plagiarism detection, and communication via well-defined
    APIs.

- One of the critical components is the plagiarism detection algorithm, employing advanced code analysis techniques and similarity
    algorithms to identify instances of plagiarism accurately.

- The user interface (UI) and user experience (UX) design focus on simplicity, responsiveness, and clear navigation,
    ensuring an intuitive and visually appealing interface for assignment submission, feedback review, and grade tracking.

- We integrate AI algorithms for automated code analysis and grading, leveraging machine learning techniques to save time
    for professors and ensure consistent evaluations.

- Our solution differentiates itself by offering a comprehensive and secure platform tailored specifically for Innopolis
    University, providing reliability, efficiency, and a user-friendly experience for code submission and grading while
    maintaining high standards of security and usability.

{{< /expand >}}

{{< hint danger >}}
**Feedback**



**Value Proposition**

Good explanation. But in the use cases you have to elaborate more. You need to give details cases how your app will be used and by whom?

**Lean startup question**

Good

**AI**

Good! But how will you do the plagiarism detection. What will you use

**Vision Of The Project**

Very good

**Overall**

The report is great, short but to the point.

5/5

_Feedback by Moofiy_
{{< /hint >}}

{{< expand "Week 2 report" >}}

**Important Note**
As the team discussions went by, we expanded our views of the project, hereby proposing new statements:

Terminology used below:

- Admin/Professor - a trusted user who can upload tasks, create contests, and view submissions from other users.
- Super-admin - part of the support team with all the admin's capabilities, plus the ability to add and remove new admins.
- Learner/User/Student - the non-privileged part of the population, who have the ability to submit tasks available to them or submit tasks from accessible contests.
- University - educational organization

**Key points about the project vision:**

 1. Provide the ability to deploy an instance of the entire project locally within the University.
    - As a subpoint, enable the creation of a zero-level admin, also known as  root, or a super-admin when deploying a custom instance.
    - Allow the integration of University's or any SSO (Single Sign-On) technology, if available, but studying the SSO technology is worthwhile.
    - Enable the option to make the project instance completely private, allowing only a limited number of users/learners from the University to access and submit tasks on the site.
    - Conversely, provide the ability to create an open platform where anyone can register and submit tasks, with super-admins adding administrators.
    - Allow the admin to add student lists with their email and group for more convenient user management. It is assumed that the University has a list of learners with their group assignments. The import format is to be discussed.
2. Create a unified configuration file for setting up the instance launch.


**Tech Stack Selection**
For stack selection it is important to note that our system is built using a microservice architecture, so we are not bound to a certain technology stack for the whole project. Now we are going to briefly explain the stack selection for the specific parts of our system:
- The service associated with testing user solutions (**orchestrator**) is built using Python, XMLRPC, Flask
- The mediator backend service (**juggler**) is build using Python, Flask, SQLAlchemy, JWT
- The database service is a standalone docker container used for storing user data - PostgreSQL
- The frontend consists of 2 services:
    - The Telegram bot - Java, Java Spring Boot
    - The on-site part - Dart, Flutter
The inter-service communication is achieved by exposing APIs. Code submission testing is believed to be secure since we are using Docker as sandboxing system.

The whole system is easily scalable and maintainable due to usage of Docker and docker-compose as build and deployment systems, also we use Prometheus and Grafana for log scrapping and visualization.

**Architecture Design**
1. Component Breakdown:
- **Orchestrator:**
    - *Responsibilities:* The orchestrator component is responsible for managing the execution of assignment submissions, test generation, and result checking.
    - *Interactions:* The orchestrator interacts with the juggler to receive assignment tasks, submissions, trigger test generation, and retrieve results.
- **Juggler (Mediator Backend Service):**
    - *Responsibilities:* The juggler component acts as a mediator between the orchestrator and other services. It handles user authentication, assignment routing, and manages communication between services.
    - *Interactions:* The juggler interacts with the orchestrator, database service, and frontend services. It receives user requests from the frontend, authenticates users, and routes the requests to the appropriate services for further processing.
- **Database Service:**
    - *Responsibilities:* The database service component is responsible for storing and retrieving user data, assignment details and other relevant information.
    - *Interactions:* The database service interacts with the juggler.
- **Frontend Services:**
    - **Telegram Bot Service:**
        - *Responsibilities:* The Telegram Bot service provides a user interface through the Telegram messaging platform. It allows users to submit assignments, receive feedback
        - *Interactions:* The Telegram Bot service interacts with the juggler. It receives assignment submissions from users, sends them to the juggler for further processing, and recieves feedback.
    - **On-Site Part:**
        - *Responsibilities:* The On-Site Part service offers an intuitive and visually appealing user interface. It allows students to submit assignments, take part in contests and access other features.
        - *Interactions:* The On-Site Part service interacts with the juggler. It receives assignment submissions, sends them to the juggler for processing, and retrieves relevant information.

![](/LeetForcesResources/LFreport2.png)
*Reference architecture diagram*

2. Data Management:
- The juggler uses databases implemented using PostgreSQL, that is responsible for storing user data and other relevant information. It ensures data integrity and provides efficient data retrieval capabilities.
3. User Interface (UI) Design:
- The frontend of the system consists of two services:
    - **The Telegram Bot Service:** Developed using Java and Java Spring Boot, this service handles user interactions through the Telegram messaging platform. It provides a user-friendly interface for users to submit assignments, receive feedback, and track their progress.
    - **The On-Site Part:** Built with Dart and Flutter, this service offers an intuitive and visually appealing interface for users to interact with the system. It allows students to submit assignments, take part in contests and access other features.

![](/LeetForcesResources/SiteDesign.jpeg)
*Site design in Figma*, [link to the design](https://www.figma.com/proto/kXwTmif6geaaXD5AuSVp1S/CODETEST?page-id=0%3A1&type=design&node-id=13-158&viewport=-3269%2C-203%2C0.57&scaling=scale-down&starting-point-node-id=13%3A158)

4. Integration and APIs:
- The microservices within the system communicate with each other through exposed APIs. This allows seamless integration and data exchange between the orchestrator, juggler, and other services, enabling efficient workflow management and assignment processing
- The integration with the Telegram API enables users to conveniently interact with the system through the Telegram messaging platform, providing a seamless user experience.
5. Scalability and Performance:
- The microservice architecture, combined with Docker and docker-compose, provides scalability and performance advantages. Each microservice can be independently scaled based on demand, ensuring optimal resource utilization and responsiveness, even under high user loads.
6. Security and Privacy:
- Security measures are incorporated into the system to protect user data and ensure privacy. Key security considerations include:
    - Authentication and authorization mechanisms to verify the identity and access rights of users and ensure secure access to sensitive data.
    - To ensure the security and stability of the system, custom processes, such as code submissions, are isolated within separate Docker sandbox containers. This isolation prevents potential malicious code or vulnerabilities from impacting the underlying system or compromising user data.
7. Error Handling and Resilience:
- The system includes robust error handling mechanisms to maintain reliability and resilience. Strategies for error logging, monitoring are implemented to ensure the system can recover from failures and maintain uninterrupted operation.
8. Deployment and DevOps:
- DevOps practices are employed to streamline the deployment process and ensure efficient collaboration among team members. Key aspects include:
    - Deployment Process:
        - *Automation:* The deployment process is automated using tools such as Docker and docker-compose. These tools enable the creation of containerized environments, making it easier to deploy the system consistently across different environments.
        - *Continuous Integration/Continuous Deployment (CI/CD):* GitHub Actions CI/CD is utilized to automate the build, testing, and deployment processes. This ensures that changes made to the codebase are thoroughly tested and seamlessly deployed to production or staging environments.
    -  Version control is managed using Git and the codebase is hosted on GitHub. This allows for efficient collaboration among team members, version tracking, and easy rollback in case of issues.
    - Monitoring and log scraping are implemented using Prometheus and Grafana. These tools provide insights into the system's performance, resource utilization, and error tracking, helping identify and resolve issues promptly.
    - Development Workflow:
        - *Collaboration:* The team follows collaborative development practices, utilizing Git branches, pull requests, dashboard and code reviews to ensure code quality and prevent conflicts.
        - *Agile and Iterative Approach:* An agile methodology is adopted, enabling iterative development, frequent releases, and the incorporation of user feedback into subsequent iterations.
{{< /expand >}}

{{< hint danger >}}
**Feedback**  

**1. Component Breakdown**

Good, 

**2. Data Management**

Good!!

**3. UI Design**

Nice designs
But the design in desktop-8 you should show how will you present the contests 

**4. Integration and APIs**

But you integrate with your own API :)

**5. Scalability and Performance**
Good

**6. Security and Privacy**
Good

**7. Error handling and Resillience**
You will do all of that? I highly doubt that it’s manageable. 
Maybe pick one or tow and focus to perfect them. 

**8. Deployment and DevOps**
Very Good

**Answering questioner**
Missing?

**Overall**
The report is  good. But you didn’t answer the questioner

Grade 4/5


_Feedback by Moofiy_
{{< /hint >}}
