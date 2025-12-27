

# StudyFlow-AIIII

Final project for the Building AI course

## Summary

StudyFlow AI is a smart scheduling tool that helps students manage study time effectively. It uses AI to recommend what to study next, predict time needed per topic, and create personalized weekly plans. By analyzing past performance and deadlines, it reduces procrastination and boosts productivity.


## Background

Which problems does your idea solve? How common or frequent is this problem? What is your personal motivation? Why is this topic important or interesting?

This is how you make a list, if you need one:
* problem 1: Inefficient time allocation – Students often study randomly rather than focusing on weak areas, wasting valuable time.
* problem 2: Procrastination and deadline overload – Without a smart schedule, students delay studying until deadlines stack up, increasing stress.


## How is it used?

A student starts by entering their subjects, deadlines, and past grades. The system then creates a personalized study schedule by comparing their data with similar learners and predicting the time needed for each topic. The student follows the daily plan, logs their progress, and the schedule adapts based on their actual performance—focusing more on weaker areas and adjusting timelines as needed.

It’s designed for busy study periods like exam weeks or project deadlines, and is aimed at students at any level who need help managing their time effectively. The tool prioritizes privacy, flexibility for different schedules, and a simple interface that encourages consistent use without adding extra stress. ![Student studying with a planner](https://images.unsplash.com/photo-1434030216411-0b793f4b4173?ixlib=rb-1.2.1&auto=format&fit=crop&w=600&q=80) 

This is how you create code examples:
```
def main():
   countries = ['Denmark', 'Finland', 'Iceland', 'Norway', 'Sweden']
   pop = [5615000, 5439000, 324000, 5080000, 9609000]   # not actually needed in this exercise...
   fishers = [1891, 2652, 3800, 11611, 1757]

   totPop = sum(pop)
   totFish = sum(fishers)

   # write your solution here

   for i in range(len(countries)):
      print("%s %.2f%%" % (countries[i], 100.0))    # current just prints 100%

main()
```


## Data sources and AI methods
The project uses both open educational datasets and self‑collected user data. Initial training data comes from public sources such as the Student Performance Data Set (UCI Machine Learning Repository), which includes grades, study time, and demographic factors. In real use, students voluntarily contribute anonymized logs of their study sessions, quiz scores, and deadlines. All personal data is stored locally or anonymized before aggregation.

The AI methods are intentionally simple and transparent:

Nearest neighbor to find students with similar performance patterns and recommend what worked for them.

Linear regression to predict the time needed to reach a target score based on past study efficiency.


These techniques were chosen because they are interpretable, easy to implement, and covered in the Building AI course—making the project a practical demonstration of foundational machine learning.

## Challenges

What the project does not solve:

Lack of motivation or self-discipline in students.

Deep conceptual learning difficulties that require expert teaching.

Non-academic factors affecting study time (e.g., health issues, work obligations).

Technical limitations:

"Cold start" problem: new users without historical data receive generic recommendations.

Overfitting risk if training data is too small or not diverse.



## What next?

To move from a prototype to a usable tool, the next steps would include:

Building a simple web or mobile interface where students can input their data and view their schedule.

Integrating with calendar APIs (Google Calendar, Outlook) to sync study blocks automatically.

Adding natural language input (e.g., “I have a biology test next Friday”) for easier setup.


## Acknowledgments

Inspired by productivity tools like Forest and Quizlet, and by the “spaced repetition” learning technique.

Dataset: Student Performance Data Set from the UCI Machine Learning Repository (public domain for academic use).

Course materials from Elements of AI provided the foundation in nearest neighbor and linear regression methods.

Unsplash image used in the README: “Desk with notebook and laptop” by Glenn Carstens‑Peters – free to use under the Unsplash License. ![Student studying with a planner](https://images.unsplash.com/photo-1434030216411-0b793f4b4173?ixlib=rb-1.2.1&auto=format&fit=crop&w=600&q=80) 

