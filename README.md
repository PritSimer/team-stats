# team-stats
codecademy//js//practice
const team = {

_players: [
  {firstName: 'John',
  lastName:   'Doe', 
  age: 25
  },
  
  {firstName: 'Jane',
  lastName:   'Smith', 
  age: 30
  },

  {firstName: 'Mike',
  lastName:   'Johnson', 
  age: 27
  }
  ],

_games: [
{opponent: 'Lions',
teamPoints: 10,
opponentPoints: 20
},
{opponent: 'Tigers',
teamPoints: 20,
opponentPoints: 30
},
{opponent: 'Dolphins',
teamPoints: 30,
opponentPoints: 10
}
],

get players(){

  return this._players
},

get games(){
   return this._games
},

addPlayer(newFirstName, newLastName,
newAge) {
  const player = {
    firstName: newFirstName,
    lastName: newLastName,
    age: newAge
  };
  this._players.push(player);
},

addGame(newOpponent, newTeamPoints, 
newOpponentPoints){
  const game = {
  opponent: newOpponent,
  teamPoints: newTeamPoints,
  opponentPoints: newOpponentPoints
};
this._games.push(game);

}
};

team.addPlayer('Bugs', 'Bunny', 76)

team.addGame('Titans', 100, 98)
console.log(team.games);
