# **CockTail**

Hi! We are team CockTail and our project is an AI which generates a cocktail based on customer's preference! Here we will publish our weekly reports with tasks we've completed during the last sprint and our goals for the next one.

<div style="text-align: center;">
<img src='/CockTail/logo.png' width="300" height="300"> 
</div>

# **Week 1**

## **Team Formation and Project Proposal**

### **Team Members**

| Team Member | Telegram ID | Email Address |
| --- | --- | --- |
| Leonid Zelenskiy | RamPrin | l.zelenskiy@innopolis.university  |
| Polina Bazhenova | poleeknow | p.bazhenova@innopolis.university |
| Ksenia Shchekina | KseniaSchekina | k.shchekina@innopolis.university  |
| Arina Yartseva | YarikaAA | a.yartseva@innopolis.university  |
| Irina Shchetinina | sch_irina73 | i.shchetinina@innopolis.university  |
| Alexander Agafonov | seoful | a.agafonov@innopolis.university  |

### **Value Proposition**

- **The problem:**
    
    Regular bar visitors often face a problem with the lack of variety of the cocktails offered by the bar list. Furthermore, a lot of bartenders, especially beginners, have difficulties with selecting ingredients for cocktails based on the customers' preferences. At the initial stage of the career, it is hard for them to remember every pair of well combined ingredients, and after a certain stage, their job for them becomes a routine and there is no place for creativity in it. Therefore, the bar list contains just few typical cocktails, and bartenders offer them to customers without taking into account their preferences. Thus, the choice of a cocktail falls entirely on an inexperienced client and the average bartender cannot help him/her.
    
- **Solution Description:**
    
    Our project will help bars varify their range of cocktails. We will create a website, the main idea of which is to complete the chain of the most suitable ingredients for the given component based on the already existing cocktail compositions from the dataset.
    
- **Benefits to Users:**
    
    Our project will help with the selection of the best ingredients for cocktails, and in addition further expand their diversity. Thus, the quality of the bar service will reach a new level.
    
- **Differentiation:**
    
    Among the popular applications there is VIVINO. One of its functions is to select the appropriate wine for the user at his/her request. However, this function is not the main one, so it does not work perfectly. In addition, this application theats exclusively to wines. We suggest an idea that will be used by bars for increasing offered assortiment.
    
- **User Impact:**
    
    The customers of such product will be bar as a company and the users will be its staff. It simplifies the work of the bartenders. As well as a qualitative increase of the assortiment will lead to an increase in profits and popularity of the institution.
    
- **User Testimonials or Use Cases:**
    - One of our early adopters, a bartender named John, shared his experience: "This tool has been a game-changer for me. I've been able to create new and exciting cocktails that I would have never thought of on my own. It's also been a hit with the customers. They love being able to try new cocktails that are tailored to their tastes."
    - In another instance, a bar owner, Lisa, reported a significant increase in customer satisfaction and repeat business after implementing our software. She said, "Our customers love the personalized experience and the variety of cocktails we now offer. It's been a great way to differentiate our bar from others in the area."
    
    These testimonials highlight the value and benefits of our software project, demonstrating its potential to enhance the bar experience for both bartenders and customers.
    
  
{{< hint danger >}}
**Feedback**  
  Can the bar use the ingredient you will advice? 
  >Among the popular applications there is VIVINO.
  
  Why you decided to examine only this app? 
  
  Theses are not Uses cases rather than Imaginary dreams! 
  Uses cases should reflect how users will use your app and in what cases.
  You should reformulate them.
 
  
_Feedback by Moofiy_
{{< /hint >}}  
    
## **Lean Startup Questionnaire**

1. What problem or need does your software project address?
    
    *Problem of choosing the cocktail ingredients*
    
2. Who are your target users or customers?
    
    *Customer of our product is bar, but direct users will be bartenders*
    
3. How will you validate and test your assumptions about the project?
    
    *We ask our users to estimate the result (cocktail)* 
    
4. What metrics will you use to measure the success of your project?
    
    *Client satisfaction, time of performance* 
    
5. How do you plan to iterate and pivot if necessary based on user feedback?
    
    *The high-rated combinations will be included to list of possible cocktails and will take account and suggested to other users*

{{< hint danger >}}
**Feedback**  

This section has very short answers and it seems you nosed it super quickly without any consideration

>We ask our users to estimate the result (cocktail)

How, exactly? There is a lot of ways ad data can be gathered. 

>Client satisfaction, time of performance
How will you measure Client satisfaction.
time of performance of what exactly?

>The high-rated combinations will be included to list of possible cocktails…

This is not a plan to pivot 


_Feedback by Moofiy_
{{< /hint >}}

## **Leveraging AI, Open-Source, and Experts**

- AI (Artificial Intelligence):
    
    *To do this task we will use NLP model for working with text. Also the dataset  of cocktails recipes that we have do not contain any information about the cocktail flavor.  For that purpose we will use OpenAI Chat-GPT source.*
    
- Open-Source:
    
    *For this moment we found several public datasets in Hugging Face. We will combine them to one and delete unnecessary information. For the backend part we choose Django library, for the frontend part Flatter, and for the model architecture Keras library.*
    
- Experts in relevant domains:
    
    *We decided to interview the employees of bar 108 as experts in this field.*
    
{{< hint danger >}}
**Feedback**  

>To do this task we will use NLP model for working with text.

What exactly your model will do? What NLP technique will you use to build the model. 
And how will use utilise text to create cocktails?


_Feedback by Moofiy_
{{< /hint >}}
    
## **Inviting Other Students**

*We decided to create the [questionary](https://docs.google.com/forms/d/e/1FAIpQLSfcoTU38QmN0moZWnntJ6nfX4XqCXoBfU2Ch17iDytjc9r2tw/viewform?usp=sf_link) about personal experiences in selecting cocktails.*

## **Defining the Vision for Your Project**
- **Overview:**
    
    Our project will direct to the domain of bar companies. Our product will produce the cocktail composition from ingredients. It will help bartenders with making cocktail for client preferences and also will solve problem of poor bar list by providing new cocktail recipes. The bar service quality will increase due to this, hence the bar business will go up.
    
- **Schematic Drawing:**
    
    {{<mermaid>}}
    
    graph TB
      U["User"] -- "Chooses Ingredients" --> M["Website/Model"]
      M -- "Selects Best Combinations" --> D["Database"]
      D -- "Checks for Complete Cocktail" --> M
      M -- "Offers Ready-Made Cocktail" --> U
      M -- "Store high-rated combination" --> D
      U -- "Rates the Combination" --> M
      linkStyle 0 stroke:#2ecd71,stroke-width:2px;
      linkStyle 1 stroke:#2ecd71,stroke-width:2px;
      linkStyle 2 stroke:#2ecd71,stroke-width:2px;
      linkStyle 3 stroke:#2ecd71,stroke-width:2px;
      linkStyle 4 stroke:#2ecd71,stroke-width:2px;
      linkStyle 5 stroke:#2ecd71,stroke-width:2px;
    
    {{</mermaid>}}
    
- **Tech Stack:**
    
    For frontend: Flutter framework
    
    For backend: Python, Django framewok
    
    For model: Keras library
    
- **Anticipating Future Problems:**
    
    Probably, during the process we can face challenges with databases combination. The learning of model also can be time consuming. To mitigate this problem we can use GPU and faster algorithms
    
- **Elaborate Explanations:**
    
    In out project we wil use NLP model to transform text data to the vectors. 
    
    Nowadays, there are no popular analogues of such idea that used in bar industry.
    
    
{{< hint danger >}}
**Feedback**  

The report is good, but you should have spent more time answering lean startup section 
4/5

_Feedback by Moofiy_
{{< /hint >}}

# **Week 2**

## **Team allocation**

- **Frontend:** Alexander Agafonov
    - Email Adress: [a.agafonov@innopolis.university](mailto:a.agafonov@innopolis.university)
    - Responsibilities: frontend architecture, frontend layout, connecting backend and frontend
    - Technologies, frameworks, and programming languages: Flutter (Dart)
- **Backend:** Leonid Zelenskiy
    - Email Address: [l.zelenskiy@innopolis.university](mailto:l.zelenskiy@innopolis.university)
    - Responsibilities: backend, deployment
    - Technologies, frameworks, and programming languages:
- **RL Model:** Polina Bazhenova, Arina Yartseva
    - Email addresses: [p.bazhenova@innopolis.university](mailto:p.bazhenova@innopolis.university), [a.yartseva@innopolis.university](mailto:a.yartseva@innopolis.university)
    - Responsibilities: preprocessing the data, creating and training the model for generating new cocktails
    - Technologies, frameworks, and programming languages: python and libraries
- **Recommendation system:** Ksenia Shchekina, Irina Shchetinina
    - Email addresses: [k.shchekina@innopolis.university](mailto:k.shchekina@innopolis.university), [i.shchetinina@innopolis.university](mailto:i.shchetinina@innopolis.university)
    - Responsibilities: content-based filtering, database expansion and characteristics creation
    - Technologies, frameworks, and programming languages: python, libraries (pandas, nympy)
 
## **Architecture Design**

1. **Data Management:**
    
     We will use preprocessed dataset
    
2. **User Interface (UI) Design:**
    
    [Here](https://www.figma.com/proto/f5bBoWz5X6MToXUkPBrnPF/Cocktail?type=design&node-id=10-27&scaling=scale-down&page-id=0%3A1) some variants of our UI are presented.
    
3. **Component Breakdown:**
    
    Our main components are: the model, UI and backend API. Since we have an ML project, the model is the most crucial component. Moreover, we will have nice UI for our users and functional API for other developers who would like to integrate our model.
    
    {{<mermaid>}}

graph TB

  U[User Interface] -- Request --> B
  B[Backend] -- Find By Preferences --> F[Filtering Algorithm]
  B -- Response --> U
  F -- Give Cocktail --> B
  F -- Find --> D[Dataset]
  B -- Ask For New Recipe --> M[RL Model]
  M -- Give Recipe --> B
  D -- Get Cocktail --> F

  linkStyle 0 stroke:#2ec,stroke-width:2px;
  linkStyle 1 stroke:#2ec,stroke-width:2px;
  linkStyle 2 stroke:#2ec,stroke-width:2px;
  linkStyle 3 stroke:#2ec,stroke-width:2px;
  linkStyle 4 stroke:#2ec,stroke-width:2px;
  linkStyle 5 stroke:#2ec,stroke-width:2px;
  linkStyle 6 stroke:#2ec,stroke-width:2px;
  linkStyle 7 stroke:#2ec,stroke-width:2px;

    
    {{</mermaid>}}
4. **Security and Privacy**

    We don't need high level of security, since we don't require any personal data. However, in future with scaling growth the more security will be needed.

5. **Integration and API**
 
    The backend part will include API thus the integration will not cause any problems.
    
## **Week 2 questionnaire** 

1. **Tech Stack Resources:** 
      
    At the current step, we do not utilize project-based books as we have enough of our own skills. Otherwise, if we need to increase our tech stack in future, we will find and study suitable books.
    
     
    
2. **Mentorship Support:** 
    
    As mentors we currently have Artem Batalov and Aleksander Lobanov, third year students. They already advised us with tech stack. And further we are planning to contact them in case of difficulties.
    
     
    
3. **Exploring Alternative Resources:** 
    
    - Documentation of torch, pandas, numpy, re libraries
    - Reinforcement Learning course from Innopolis Universty
    - [stackoverflow.com](http://stackoverflow.com), [geeksforgeeks.org](http://geeksforgeeks.org)
    
     
    
4. **Identifying Knowledge Gaps:** 
    
    At the moment, we are not experiencing difficulties in the knowledge of the technical stack we need. Otherwise, if there is a lack of knowledge or experience, we will ask teammates for the help, or if it is a more serious problem, then we will turn to scientific papers and documentation.
    
     
    
5. **Engaging with the Tech Community:** 
    
    We do not actively engage with the broader tech community to seek guidance or learn from seasoned professionals in our tech stack. In case of critical tech stack problems, we will use online forums, but at current stage of the work we do not need this.
    
     
    
6. **Learning Objectives:** 
    
    - One of our objectives is to study papers about usage of models for predicting the sequence of elements.
    - Another one is to find the most suitable frameworks for our project.
    - Also our objective is the deep studying of filtering algorithms and finding the one that most fits for our purpose
    
     
    
7. **Sharing Knowledge with Peers:** 
    
    We have created team chat in telegram, where we can discuss thoughts and ideas. In addition, weekly we have face-to-face meetings to share knowledge and expertise with each other.
    
     
    
8. **AI leveraging:**

     We leveraged OpenAI for the quick search of some functions usage and for characteristics generation.
     
## **Weekly Progress Report**

Over the past week there is changes in our project plan. We decided to make the recommendation system for the users based on the filters. Besides that, we concluded that NLP model is quite complex for our problem and to avoid overfitting it is better to utilize simpler one.

As of the progress in our project, we have found a suitable dataset and finished its preprocessing. Also, we have developed a design for the future web application. In addition, we explored the materials on cocktail theory and interviewed some prospective experts in order to dig deeper into the main idea of our project.

We’ve designed different variants of UI, but didn’t decided which to choose. Also we are planning to change backend stack from Django to FastAPI, since there’s no need for such functional framework. 
