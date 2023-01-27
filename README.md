# Website Documentation
Welcome to our website documentation!
For some reason such as the privacy agreement, we cannot publish the source code to the public.

## Website Introduction
Our website, Authentic Animal Auscultation, is a training website for vets as well as vet students. 
The inspiration of our website is that our client, the vet school of Bristol University, has found that most newly graduated vets make no evident progress in animal auscultation skills after graduation. Although the vets received training in auscultation during their studies in the final year of vet school, many of them do not insist on learning auscultation after they graduated. The vet school believes that the solution to this problem is encouraging the vets to listen to sounds from different animals repeatedly. Therefore, an idea to build a website delivering training resources arose. We believe that this can not only help Bristol newly graduated vets, but also worldwide vet students, vet professionals.

## Key Features
Our clients expects that a user can search for some terminologies to listen to corresponding animal sounds, take quizzes to test their knowledge, and watch some tutorial videos on the website. To fulfill the above-mentioned needs, the structure of the website is designed as below.

### Website Structure Diagram

.
└── Home Page  
    ├── Library & Search Page  
    │   └── Search Result List Page  
    │       └── Result Content Page  
    │  
    ├── Self-test Page  
    │  
    ├── Tutorial Page  
    │  
    ├── My Account Page  
    │   └── My Collection Page  
    │  
    └── Admin Management System  
.


### Website Functionality
In the home page of our website, a user can sign up or login using the My Account button on the upper corner of the page. The user can also choose to use the library & Search module or the Self-test module or the Tutorial module from the three biggest buttons in the middle of the page.
#### Library & Search module
In the search bar of the Library & Search module, a user can search for terminologies by typing keywords. This can return a list of existing terminologies that contain the keyword in their title or description fields. The Search Result List page will be opened to display the list. If the list contains too many results, pagination can divide these results into several pages. In the Search Result List Page, the user can click one of the results to study the content of the terminology.
Moreover, a collection function is built based on the Result Content page. This feature enables the logged-in users to add terminologies to their collection list.
#### Self-test Page
The Self-test page lists some multiple-choice questions. A logged-in user can take the self-test quiz to test their auscultation skills.
#### Tutorial Page
The Tutorial page lists some tutorial videos. A user can watch the videos to better understand the practice of auscultation.
#### Admin Management System
We also include a backstage Admin Management System. If the client logins as an admin role user, the client can update and manage the website on their own in this system.

## Repository Structure
In this project, we separate front-end and back-end.
We apply Html5+CSS+JavaScript as front-end technologies and Java with SQL database as back-end technologies. In the front-end development, we use VUE framework. Relevant code can be found in the web folder. In the back-end development, we use SpringBoot framework. Relevant code can be found in the src folder. 
As we build java project with Maven, our project can be tested by DemoApplicationTests.java in the test folder. Moreover, the configuration information is included in the pom.xml file.

. 
├── .idea
│
├── node_modules
│
├── src
│   ├── main
│   │   └── java.com.mastercs.demo
│   │       ├── bean
│   │       │   ├── EnumOption.java
│   │       │   ├── EnumRole.java
│   │       │   ├── FavorRecords.java
│   │       │   ├── Knowledge.java   
│   │       │   ├── Options.java
│   │       │   ├── Question.java
│   │       │   ├── Result.java
│   │       │   ├── Role.java
│   │       │   ├── Search.java
│   │       │   ├── Tutorial.java
│   │       │   ├── User.java
│   │       │   └── UserQuestion.java   
│   │       │             
│   │       ├── config
│   │       │   ├── CorsConfig.java
│   │       │   ├── MybatisPlusConfig.java
│   │       │   └── SpringMvcConfig.java
│   │       │
│   │       ├── controller
│   │       │   ├── AdminController.java
│   │       │   ├── AuthController.java
│   │       │   ├── ContentController.java
│   │       │   ├── FilesController.java
│   │       │   ├── QuizController.java
│   │       │   ├── SearchController.java
│   │       │   └── TutorialController.java
│   │       │
│   │       ├── exception
│   │       │   └── GlobalExceptionHandler.java
│   │       │
│   │       ├── mapper
│   │       │   ├── FavorRecordsMapper.java
│   │       │   ├── KnowledgeMapper.java
│   │       │   └── TutorialMapper.java
│   │       │
│   │       ├── payload
│   │       │   ├── AdminAddDto.java
│   │       │   ├── AdminDeleteDto.java
│   │       │   ├── AllQuizResponse.java
│   │       │   ├── KnowledgeDto.java
│   │       │   ├── LoginDto.java
│   │       │   ├── LoginResponse.java
│   │       │   ├── ModifyQuizDto.java
│   │       │   ├── PageInfo.java
│   │       │   ├── QuestionResponse.java
│   │       │   ├── Receive.java
│   │       │   ├── SignupDto.java
│   │       │   └── TutorialDto.java
│   │       │ 
│   │       ├── repository
│   │       │   ├── OptionRepository.java
│   │       │   ├── QuestionRepository.java
│   │       │   ├── RoleRepository.java
│   │       │   ├── SearchDAO.java
│   │       │   ├── SearchDAO2.java
│   │       │   ├── UserQuestionRepository.java
│   │       │   └── UserRepository.java
│   │       │   
│   │       ├── services
│   │       │   ├── impl 
│   │       │   │   └── interceptor 
│   │       │   │       ├── LoginInterceptor.java
│   │       │   │       └── PermissionInterceptor.java
│   │       │   ├── KnowledgeServiceImpl.java
│   │       │   └── TutorialServiceImpl.java
│   │       │
│   │       ├── utils
│   │       │   └── JwtUtils.java
│   │       │
│   │       ├── DemoApplication.java
│   │
│   ├── test
│       └── java.com.mastercs.demo
│           └── DemoApplicationTests.java
│
├── target
│
├── web
│
├── mvnw
│
├── mvnw.cmd
│
├── package.json
│
├── pom.xml
│
└── README.md
.

## Version Documentation
We have mainly maintained 2 versions of the project in GitHub due to agile development.
|  version   |                   features                             |  link   |
|   ----     |                    ----                                |  ----   |   
|     1      |            Library & Search, Self-test                 |         |
|     2      | add Tutorial, My Collection, Admin Management System   |         |

## Quick Start Guide
The guide shows how to run our project on your computer. We recommend using IntelliJ IDEA to open this project.
### Step 1. Preparation
If you open the project by IntelliJ IDEA, the pom.xml file will automatically download all dependencies to build the project.
### Step 2. Run
You can run the project by DemoApplication.java in the src folder.
You can open http://localhost:8888 to view web pages in your browser. 



