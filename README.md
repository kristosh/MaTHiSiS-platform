# Instructions.

Instructions about e-learning platform.

## Installation

Just right click the .jar file and the app will start.

```
mathisis.jar
```

Or from a command line:

```
java -jar mathisis.jar
```

## About the platform.

The testbed platform used in our study is a serious game called Learnin platform developed specifically 
for the purposes of this research from Maastricht University. 
The platform consists of two major functionalities: 

* The teacher account functionality, 
with which tutor has the ability to add new subjects and questions of varying types, 
levels of difficulty and  also tune maximum available time for the answer to be given by the student, 
* The student account functionality which performs the learning sessions of Learnin platform. 
The learner entering with student credentials can choose between 4 different default subjects (Math, Sports, Geography, History). 
For the purpose of data acquisition, every time the learner is playing a specific subject, 
the level of difficulty is changing randomly. The levels of difficulty are in total 9 (from 1-9). 
Throughout the learning session, the learner is informed about the current level, the current 
score and the time left for answering the question. A detailed description of the 
testbed platform interfaces is the following:

### Teacher interfaces:

* When the user presses the tutor scene button, the learning platform directs to the tutor scene and the Log in/Sign up interface is prompted.
* Then, tutor logs in or, in the case that an account has not been created, the sign up process must be performed. In the sign up screen, the user adds information in order to create an account and to be able to log in to the system.
* Consequently, the game directs tutor to the add new material scene. Here, the tutor has two options. To add new subjects or to add new questions.
* If the tutor chooses to add a new subject, then the name of it needs to be added accordingly.
* In the case that the tutor chooses to add a new question, s/he has to select the type of the question to be included. In the learning platform, three different types of questions are available: choose an answer, true or false and open answer questions (requires from the learner to enter the whole answer). 
* Finally, the rest of the information related to the question has to be provided. This information includes  the maximum available time for the learner, its level of difficulty and, in the case of 'choose an answer' question, the possible fake answers which are called distractors.
* In the case that the tutor chooses to add a new question, s/he has to add the content and the type of the question, the maximum available time for the learner, the level of difficulty and the possible fake answers in case the question belongs to the category 'choose an answer'
* There are three different types of questions: choose an answer, true or false and open answer questions (requires from the learner to enter the whole answer). 

### Student interfaces:

   * An introduction interface, where the two different accounts (teacher and student) are presented 
in two different buttons.
   * When the learner presses the student scene button, the Log in/Sign up interface is presented.
   * Students add their information (demographics) in sign up scene in order to be able to login.
   * Subsequently, students are directed to subject interface where they can choose a subject among 
4 different courses ('Math', 'History', 'Sports', 'Geography') and then they can start a new game.
   * Then, the learning session begins and the learners have to answer 7 different questions.
   * During the learning session, questions, the possible answers and a status bar with information 
for the learning session is rendered to the learner.
   * There are three different types of questions: choose an answer, true or false, introduce an 
answer (requires from the learner to enter the whole answer). 
   * During the learning sessions, different sounds and emoticons are used with scope to provoke 
and boost learners reactions.
   * After each session, learners were asked to annotate their affective states, levels of engagement, 
boredom and frustration in scale of 0-5.
   * The next scene is the result panel interface, which informs learners about their performance 
during the session.
   * Finally, learner has the choice to either logout or continue with a new session. In the latter case, 
learner has to choose a subject and to start the new session.
   * Teacher interfaces are not presented since this is out of the scope of this study.

### Dataset

This platform mainly was developed in an effort to created a leanring dataset. That dataset consists of students from Maastricht University, the Netherlands, voluntarily playing the 'learning platform'. The dataset is available for download after communication with the authors, through the dedicated form found in the following link:v https://project.dke.maastrichtuniversity.nl/kristosh/index.php.

The learners were bachelor and master students (with a mean age of 22.6 years and standard deviation of 3.1), from two different knowledge profiles, namely software engineering and psychology. Each student performed four learning sessions in each of the four available subjects. After every learning session, the users were asked to assess, on a Likert scale (from zero to five), the degree of engagement, frustration and boredom variables that they experienced. The analysis presented in this paper was based on 33 players (16 males and 17 females). The lighting conditions during the capturing procedure were typical for an office environment and a web camera was used for capturing facial and upper torso expressivity. The detailed description for the data acquisition protocol is the following:

* A consent form was given to every participant. This form contains all the information needed, for the students to understand the reason behind the experiment and the gathering of the data. The content of this consent form was reviewed and approved by the Ethical Review Committee of Maastricht University. 
* Additionally, oral instructions were given to the participants with  information about the process that they had to follow. 
* Participants were told that throughout the experiment they will have to play 16 different learning sessions in total.
* Due to time constraints, students were played just 4 sessions per each subject.
* The duration for the whole experiment per each participant was 26±5 minutes.
* The system automatically changed the difficulty levels based on the performance of the learners. 
* The reason behind this, was to record information from as many difficulty levels as possible and analyze afterwards as a function of experienced emotion and user profile.
* In order to facilitate the experiments' performance and avoid users feeling tired (thus, biasing acquired data), it was decided to establish a restriction per subject so that the learner only performed tests belonging to four out of nine levels. However, to record data belonging to all difficulty levels without exceeding the time constraint (around 30 minutes per each participant to perform the whole experimental phase), the approach implemented was dependent on the score achieved in the previous session. At the beginning, the first level was established randomly between levels one and three (out of nine). Subsequently, the increase of the level was based on the score obtained by the user. In this way, the user was asked to answer questions related to levels four or five, six or seven and eight or nine, depending on whether or not the learner's score would reach a certain threshold. The whole procedure led to sparse matrices of learners and difficulty levels which are suitable for the performed study done and described in the experimental results.

The 'learning platform' contains two databases. Firstly, a database which contains all of the default provided questions of the platform. This database consists of a unique table which includes the following fields:

* **questionID**: This field contains the unique identities (id) for every question in order to be easily retrieved from the dataset of the platform.
* **subject**: It is the subject of the question.
* **type**: This field contains the type of the question (choose an answer, true or false and introduce an answer).
* **level**: It is the difficulty level of the question.
* **time**: The field speed contains the maximum available time for each question (in seconds).
* **question**: This field contains the question content.
* **answer**: It is the correct answer of the question.
* **fake1, fake2**:  In the case of 'choose an answer' questions, these two extra fields are used to incorporate the distractors for the question, which were introduced from the tutor using the tutor profile. 

Secondly, the platform contains the user database which incorporates all the information about the interactions of the learners with the platform during the learning sessions. This database contains 5 different tables: 

* StudentsInfo.
* StudentsLevel. 
* StudentsQuestion. 
* StudentsScore. 
* StudentsSession.

StudentsInfo table consists of the demographics of the learner as filled up during the sign-up stage. A detailed description of the fields of this table is as follows: 

* **userID**: A unique identity which is assigned to every user.
* **name, surname**: The name and surname of the user.
* **username, password**: The username and the password that the user choose during the sign up process and they are used as crendentials in order to be able to login in the game.
* **age, gender**: Those fields contain the basic demographic fields, which were filled in by the user.
* **knowledge, department**: Those fields contain learner's knowledge background (high school, bachelor, master and PhD) and learner's department (engineering, psychology).
* **subject annotated level**: This field corresponds to the learner's self-evaluation of their skill level on each of the four presented subjects.
\end{itemize}

Table StudentsLevel contains information about the employed difficulty level in all of the available subjects and it is used by the system to conduct the appropriate flow in subsequent learning sessions. Table StudentsScore contains the score obtained for each learner and subject. StudentsQuestions contains information about each learner's answer to the prompted questions for all of the learning sessions performed. In particular, the fields that this table includes are:


* **userID**: The identity of the user that answers a specific question.
* **sessionID**: The identity of the specific session in which this question was asked. 
* **questionID**: The identity of the corresponding question.
* **date**: A timestamp that illustrates the exact time when the question was answered.
* **course**: The name of the course of the question.
* **level**: The level of difficulty of the question.
* **time**: The total amount of time that the user needed for answering the question.
* **answer**: This field shows whether or not the user answered the question and if so, whether or not the correct answer was given.


Finally, the StudentsSession table contains all the related information for every learning session. It contains the following fields:

* **sessionID**: The unique identity of a specific learning session. 
* **userID**: The identity of the user when interacted with the specific session.
* **date**: A timestamp that illustrates the exact time that the corresponding learning session began.
* **course**: The name of the course of the corresponding session.
* **level**: The level of difficulty of the corresponding session.
* **trial**: An indicator that shows how many times the user has previously interacted with a specific course.
* **score**: The field score represents the number of the correct answers of the user during the corresponding session.
* **boredom-assessment, engagement-assessment, frustration-assessment**: It is the self-annotation of the users that they provided after the end of each learning session and corresponds to the level of engagement, boredom and frustration that the learner felt during the corresponding session respectively.

# The flow of the learning platform for the learner
## Choose a role panel
![choose_a_role](https://user-images.githubusercontent.com/24369160/65315465-7373ed80-db98-11e9-896a-8832cb8f8f5a.JPG)
## Sign up panel
![sign_up_learner](https://user-images.githubusercontent.com/24369160/65315535-90102580-db98-11e9-8be6-cb88c75e9121.JPG)
## Login panel
![Capture1](https://user-images.githubusercontent.com/24369160/61784307-c5eb9480-ae09-11e9-8ef7-d44b17324eeb.PNG)
## Choose a course panel
![capture6](https://user-images.githubusercontent.com/24369160/65252215-dada6080-daf8-11e9-8ecf-f974fc8c8efe.png)
## Question panel
![Capture](https://user-images.githubusercontent.com/24369160/61784305-c552fe00-ae09-11e9-9870-6ee133a35814.PNG)
## Questionnaires
![Capture8](https://user-images.githubusercontent.com/24369160/65259362-d2882280-db04-11e9-9455-3b45192a3ab0.JPG)
## Results panel
![Capture6](https://user-images.githubusercontent.com/24369160/65251343-7539a480-daf7-11e9-806e-876ae585fe2f.JPG)

# The flow of the learning platform for the tutor
## Sign up panel
![teacher_sign_up](https://user-images.githubusercontent.com/24369160/65315607-afa74e00-db98-11e9-84eb-804ae429c17f.JPG)
## Tutor panel
![teacher_panel](https://user-images.githubusercontent.com/24369160/65315618-b5049880-db98-11e9-8172-9a1217199529.JPG)


