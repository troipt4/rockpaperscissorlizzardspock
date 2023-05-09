# rock_paper_scissor_lizzard_spock

#include <iostream>
#include <stdlib.h>
using namespace std;

int main(){
  /* The different outcomes:
  scissors cuts paper
  paper covers rock
  rock crushes lizard
  lizzard poisons spock
  spock smashes scissors
  scissors decapitate lizzard
  lizzard eats paper
  paper disproves spock
  spock vaporizes rock
  rock crushes scissors*/
  srand (time(NULL));
  int computer = rand() % 3 + 1;
  int user = 0;


cout << "====================\n";
cout << "rock paper scissors!\n";
cout << "====================\n";
 
cout << "1) Rock\n";
cout << "2) Paper\n";
cout << "3) Scissors\n";
cout << "5) Lizzard\n";
cout << "4) Spock\n";
 
cout << "Shoot! ";
cin >> user;

if (user == 1)
    cout << "you choose: ✊\n";
  else if (user == 2)
    cout << "you choose: ✋\n";
  else if (user == 3)
    cout << "you choose: ✌️\n";
   else if (user == 4)
    cout << "you choose: 🦎\n";
  else
    cout << "you choose: 🖖\n";

  if (computer == 1)
    std::cout << "cpu choose: ✊\n";
  else if (computer == 2)
    std::cout << "cpu choose: ✋\n";
  else
    std::cout << "cpu choose: ✌️\n";



if (user == computer) {

    std::cout << "it's a tie!\n";

  }

  // user rock

  else if (user == 1) {

    if (computer == 2) {

      std::cout << "you lost! booooo!\n";

    }
    if (computer == 3) {

      std::cout << "you won! woohoo!\n";

    }

  }

  // user paper

  else if (user == 2) {

    if (computer == 1) {

      std::cout << "you won! woohoo!\n";

    }
    if (computer == 3) {

      std::cout << "you lost! boo!\n";

    }

  }

  // user scissors

  else if (user == 3) {

    if (computer == 1) {

      std::cout << "you won! woohoo!\n";

    }
    if (computer == 2) {

      std::cout << "you lost! booooo!\n";

    }
  }
  //user 
}


