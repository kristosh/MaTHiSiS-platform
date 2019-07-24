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
* Consequently, the game directs tutor to the add new material scene. Here, the tutor has two options. To add new subjects or to add new questions.}.
* If the tutor chooses to add a new subject, then the name of it needs to be added accordingly.
* In the case that the tutor chooses to add a new question, s/he has to select the type of the question to be included. In the learning platform, three different types of questions are available: choose an answer, true or false and open answer questions (requires from the learner to enter the whole answer). 
* Finally, the rest of the information related to the question has to be provided. This information includes  the maximum available time for the learner, its level of difficulty and, in the case of ``choose an answer'' question, the possible fake answers which are called distractors.
* In the case that the tutor chooses to add a new question, s/he has to add the content and the type of the question, the maximum available time for the learner, the level of difficulty and the possible fake answers in case the question belongs to the category ``choose an answer''
* There are three different types of questions: choose an answer, true or false and open answer questions (requires from the learner to enter the whole answer). 

### Student interfaces:

   * An introduction interface, where the two different accounts (teacher and student) are presented 
in two different buttons.
   * When the learner presses the student scene button, the Log in/Sign up interface is presented.
   * Students add their information (demographics) in sign up scene in order to be able to login.
   * Subsequently, students are directed to subject interface where they can choose a subject among 
4 different courses (``Math'', ``History'', ``Sports'', ``Geography'') and then they can start a new game.
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



# Login screenshot
![Capture](https://user-images.githubusercontent.com/24369160/61784305-c552fe00-ae09-11e9-9870-6ee133a35814.PNG)
# Question screenshot
![Capture1](https://user-images.githubusercontent.com/24369160/61784307-c5eb9480-ae09-11e9-8ef7-d44b17324eeb.PNG)
