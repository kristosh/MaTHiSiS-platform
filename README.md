# Instructions.

Instructions about e-learning platform.

## Installation

Just right click the .jar file and the app will start.

```mathisis.jar
```

## About the platform.

The testbed platform used in our study is a serious game called ``Learnin' platform'' developed specifically 
for the purposes of this research from Maastricht University. The original ``Learnin' platform'' 
is available on Github\footnote{https://github.com/kristosh/Mathisis-platform}. 
The platform consists of two major functionalities: 1. The teacher account functionality, 
with which tutor has the ability to add new subjects and questions of varying types, 
levels of difficulty and  also tune maximum available time for the answer to be given by the student, 2. 
The student account functionality which performs the learning sessions of ``Learnin' platform''. 
The learner entering with student credentials can choose 
between 4 different default subjects (``Math'', ``Sports'', ``Geography'', ``History''). 
For the purpose of data acquisition, every time the learner is playing a specific subject, 
the level of difficulty is changing randomly. The levels of difficulty are in total 9 (from 1-9). 
Throughout the learning session, the learner is informed about the current level, the current 
score and the time left for answering the question. A detailed description of the 
testbed platform interfaces is the following:

```
- An introduction interface, where the two different accounts (teacher and student) are presented 
in two different buttons, (Fig. \ref{fig:lp1}).
- When the learner presses the student scene button, the Log in/Sign up interface is presented.
- Students add their information (demographics) in sign up scene in order to be able to login.
- Subsequently, students are directed to subject interface where they can choose a subject among 
4 different courses (``Math'', ``History'', ``Sports'', ``Geography'') and then they can start a new game.
- Then, the learning session begins and the learners have to answer 7 different questions 
(Fig. \ref{fig:lp2}).
- During the learning session, questions, the possible answers and a status bar with information 
for the learning session is rendered to the learner.
- There are three different types of questions: choose an answer, true or false, introduce an 
answer (requires from the learner to enter the whole answer). 
- During the learning sessions, different sounds and emoticons are used with scope to provoke 
and boost learners reactions.
- After each session, learners were asked to annotate their affective states, levels of engagement, 
boredom and frustration in scale of 0-5.
- The next scene is the result panel interface, which informs learners about their performance 
during the session.
- Finally, learner has the choice to either logout or continue with a new session. In the latter case, 
learner has to choose a subject and to start the new session.
- Teacher interfaces are not presented since this is out of the scope of this study.
```