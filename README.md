# TriviaGame
<!DOCTYPE html>
<html>
    <head> 
        <Title>Totally Trivial Trivia</Title>
        <link href="style.css" rel="stylesheet">
    </head>
    <body>
        <div id = "quizContainer" class = "container"> 
            <div class = "Title"> Totally Trivial Trivia</div>
            <div id = "question" class = "question"></div>
            <label class ="option"><input type = "radio" name = "option" value = "1" /> <span id="opti1"></label>
            <label class ="option"><input type = "radio" name = "option" value = "2" /> <span id="opti1"></label>
            <label class ="option"><input type = "radio" name = "option" value = "3" /> <span id="opti1"></label>
            <label class ="option"><input type = "radio" name = "option" value = "4" /> <span id="opti1"></label>
            <button id = "nextButton" class="next-btn" onclick="loadNextQuestion();">Next Question</button>
        </div>
        <div id="result" class="container result" style="display:none;">
        </div>
        <script src="app.js"></script>
        <script src="quiz.js"></script>

    </body>
</html>

var questions = [{
    "question": "How many states are in the United States?",
    "option1": "51"
    "option2": "50"
    "option3": "20"
    "option4": "25"
    "answer": "50"
}, {
    "question": "Who invented the light bulb?",
    "option1": "Thomas Edison"
    "option2":  "Benjamin Franklin"
    "option3":  "Einstein"
    "option4":  "Henry Ford"
    "answer" : "Thomas Edison"
}

body { 
    font-family: 'Crimson Text', serif;
    background: maroon
}
.container {
    height: 330px;
    width:  1000px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translateX(-50%) translateY(-50%);
    background: rgba(255,255,255,0.5);
    padding: 20px;
    border: 1px solid #08038c;
    box-shadow: 0 0 8px 3px #fff;
}

.title{
    padding-top: 20px;
    text-align: center;
    font-size: 36px;
    text-transform: uppercase;
    color: #08038C;
}
.question{
    padding:20px;
    font-size:22px;
    background: rgb(167, 170, 14);
    border-radius: 20px;
    margin: 10px 0 10px 0;
    color:  #f6f6f6;
}
.option{
    width: 470px;
    display: inline-block;
    padding: 10px 0 10px 15px;
    vertical-align: middle;
    background: rgba (255,255,255,0.5);
    margin: 10px 0 10px 10px ;
    color: black;
    border-radius: 20px
    
}
.option:hover{
    background: #08038c;
    color: #f6f6f6;

}

.next-btn{
    border: none;
    outline: none;
    background: rgba (255,25,255,0.5);
    width: 100px;
    height:35px;
    border-radius: 20px;
    cursor: pointer;
    float:right;
    margin: 10px;
}

.next-btn:hover{
    background: #08038C
    color: #f6f6f6;
}

.result{
    height: 100px;
    text-align: center;
    font-size: 75px;

}

.option input:checked.option{
    background: #08038C
    color: #000;
}
