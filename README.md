# GnosisColosseum

Data structure for quiz
```
    struct Quiz {
        address creator;        // creator of quiz
        bytes32 quizAnswerHash; // store correct answer hash in storage
        uint price;             // min price to guess the word
        uint pledged;           // pledged amount 
        uint startAt;           // default block.timestamp (current time)
        uint endAt;             // max 90 days
        string uri;             // uri for quiz.It contains question ,description and image etc.
        address winner;         // winner of the quiz.If a quiz has a winner wouldn't users guess and creator can't claim pledged money.
    }
```