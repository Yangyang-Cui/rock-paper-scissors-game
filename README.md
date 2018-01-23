# rock-paper-scissors-game
rock paper scissors game( codecademy)

const getUserChoice = (userInput) =>{
  userInput = userInput.toLowerCase();
  if ( userInput === 'rock' || userInput ==='paper' || userInput === 'scissors') {
    return userInput;
  } else {
    console.log('You type wrong message.');
  }
}

let getComputerChoice = () => {
  numberRandom = Math.floor(Math.random()*3);
  switch (numberRandom){
    case 0:
      'rock';
      break;
    case 1:
      'paper';
      break;
    default:
      'scissors';
      break;
                      }
}

let determineWinner = (userChoice, computerChoice) =>{
  if (userChoice === computerChoice) {
    return 'Game was a tie.';
  }
    
  if (userChoice === 'rock') {
    if (computerChoice === 'scissors') {
      return 'User won.';
    }else {
      return 'Computer won.';
    }
  }
  
  if (userChoice === 'scissors'){
    if (computerChoice === 'paper'){
      return 'User won.';
      
    }else {
      return 'Computer won.';
    } 
  }
  
  
  if (userChoice === 'paper') {
 	 if (computerChoice === 'rock'){
    return 'User won.';
   } else {
    return 'Computer won.';
   }
  }
  
  let playGame = () =>{
    let userChoice = getUserChoice('rock');
    let computerChoice = getComputerChoice();
    console.log('You threw: '+ userChoice);
    console.log('The computer threw: '+computerChoice);
    determineWinner = (userChoice, computerChoice) =>{
      console.log()
    }
  }
  
  
