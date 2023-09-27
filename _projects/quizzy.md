---
layout: page
title: Quizzy
description: A quizbot that extracts topic of interest from the user and quizzes them on it.
img: assets/img/quizzy/quizbot.jpg
importance: 4
github: https://github.com/piyush-jaiswal/quizzy
---

A quizbot that extracts topic of interest from the user and quizzes them on it.

- Gets data from user responses in natural language, to find a specific topic of interest
- Engages the user in an interactive quiz
- Scores +1 for correct answer and -0.25 for wrong answer
- Ability to change the topic of interest for the quiz
- Detects ambiguous responses


<div class="row justify-content-sm-center">
    <div class="col-sm6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/quizzy/workflow.jpg" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <b><i>Workflow</i></b>
</div>

The user starts interacting with Quizzy.
- Quizzy tries to find the area of interest, on which user wants to take the quiz.
- Once the quiz topic is decided, user is quizzed on it, this is phase 2.
- User takes the quiz and is shown questions fetched from the question bank.
- User answers the questions in natural language, from which the answer is extracted and is checked against the correct option in the question bank.
- Once the quiz is complete and the user is satisfied, the user will be redirected to the initial phase i.e, phase 1.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/quizzy/2.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<!-- <div class="caption">
    <b><i>On the way to the coffee shop</i></b>
</div> -->

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/quizzy/3.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<!-- <div class="caption">
    <b><i>On the way to the coffee shop</i></b>
</div> -->

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/quizzy/4.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <b><i>Quiz flow</i></b>
</div>

Commands
- `@list_quizzes` - Displays the quiz topics available. Only applicable when selecting a quiz topic
- `@stop_quiz` - Stops the quiz and displays the final score
- `@change_quiz` - Change quiz topic. Applicable when a quiz topic is already active

<div style="margin-top: 4%;">
    <b>Project:</b> <a target="_blank" href="https://github.com/piyush-jaiswal/quizzy">https://github.com/piyush-jaiswal/quizzy</a>
</div>
