# Built-a-game-Guess-my-Number-
let  secretnumber = Math.trunc(Math.random() * 20) + 1;
let score = 20;
let highscore = 0;
document.querySelector('.number').textContent =secretnumber;

document.querySelector('.check').addEventListener('click', function () {
 const guess = Number (document.querySelector('.guess').value);
 console.log(guess, typeof guess);
 
 // when there is no input 
 
if ( !guess) {
    document.querySelector('.message').textContent ='⛔️ No number!';
    
// when player wins
} else if (guess === secretnumber) {
    document.querrynumber('.message').textcontent = 'Correct number';
    
    document.querySelector('body').style.backgroundColor = '#60b347';
    
    document.querySelector('.number').style.width ='30 rem';
    
    if(score > highscore) {
        highscore = score;
        documment.queryscore('.highscore').
        textContent = highscore;
    }
    
    // when guess is too high 
} else if (guess > secretNumber) {
  if (score > 0) {
    document.querySelector('.message').textcontent = 'Too high!;'
} else {
    document.queeySelector('.score').textContent = 'You lost the game!';
    document.querySelector('.score').textContent = 0;
    
    // when guess is too low
}
} else if (guess < secretNumber) {
    document.querySelector('.message').textContent = ' Too low!';
    score--;
    document.querySelector(.''score').textContent = score;
  }
}
});

document.querySelector('.again').addEventListener('click , function'()
score = 20;
secret number = Math.trunc('.message').textcontent = 'Start guessing;
document.querySelector('.score').textcontent = score;
document.queryselector('.number').textcontent = '?';
document.querySelector('.guess').value = '';

document.querySelector('body').style.
backgroundColor = '#222';
document.querySelector('.number').style.width = '15rem';
