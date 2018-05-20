#include <iostream>
#include <ctime>
#include <cstdlib>
#include <string>

void show_winner(char user_move, char comp_move)
{
    using namespace std;

    switch (user_move) {
        case 'r':
            switch (comp_move) {
                case 'r':
                    cout << "User: Rock" << endl;
                    cout << "Computer: Rock" << endl;
                    cout << endl;
                    for (time_t t = time(0) + 1; time(0) < t;) {}
                    cout << "Tie!" << endl;
                    break;
                case 'p':
                    cout << "User: Rock" << endl;
                    cout << "Computer: Paper" << endl;
                    cout << endl;
                    for (time_t t = time(0) + 1; time(0) <t;) {}
                    cout << "Computer Wins! Paper Beats Rock!" << endl;
                    break;
                case 's':
                    cout << "User: Rock" << endl;
                    cout << "Computer: Scissor" << endl;
                    cout << endl;
                    for (time_t t = time(0) + 1; time(0) < t;) {}
                    cout << "User Wins! Rock Beats Scissors!";
                    break;
            }
            break;
        case 'p':
            switch (comp_move) {
                case 'r':
                    cout << "User: Paper" << endl;
                    cout << "Computer: Rock" << endl;
                    cout << endl;
                    for (time_t t = time(0) + 1; time(0) < t;) {}
                    cout << "User Wins! Paper Beats Rock!" << endl;
                    break;
                case 'p':
                    cout << "User: Paper" << endl;
                    cout << "Computer: Paper" << endl;
                    cout << endl;
                    for (time_t t = time(0) + 1; time(0) < t;) {}
                    cout << "Tie!" << endl;
                    break;
                case 's':
                    cout << "User: Paper" << endl;
                    cout << "Computer: Scissors" << endl;
                    cout << endl;
                    for (time_t t = time(0) + 1; time(0) < t;) {}
                    cout << "Computer Wins! Scissors Beats Paper!" << endl;
                    break;
            }
            break;
        case 's':
            switch (comp_move) {
                case 'r':
                    cout << "User: Scissors" << endl;
                    cout << "Computer: Rock" << endl;
                    cout << endl;
                    for (time_t t = time(0) + 1; time(0) < t;) {}
                    cout << "Computer Wins! Rock Beats Scissors!";
                    break;
                case 'p':
                    cout << "User: Scissors" << endl;
                    cout << "Computer: Paper" << endl;
                    cout << endl;
                    for (time_t t = time(0) + 1; time(0) < t;) {}
                    cout << "User Wins! Scissors Beats Paper!" << endl;
                    break;
                case 's':
                    cout << "User: Scissors" << endl;
                    cout << "Computer: Scissors" << endl;
                    cout << endl;
                    for (time_t t = time(0) + 1; time(0) < t;) {}
                    cout << "Tie!" << endl;
                    break;
            }
            break;
    }
}

void countdown()
{
    using namespace std;

    // Print countdown, and wait one second after
    // each statement prints.
    cout << "Rock..." << endl;
    for (time_t t = time(0) + 1; time(0) < t;) {}
    cout << "Paper..." << endl;
    for (time_t t = time(0) + 1; time(0) < t;) {}
    cout << "Scissors..." << endl;
    for (time_t t = time(0) + 1; time(0) < t;) {}
    cout << endl;
    cout << "Shoot!" << endl;
    for (time_t t = time(0) + 1; time(0) < t;) {}
}

char get_comp()
{
    // Seed the RNG
    srand(time(NULL));

    // Divide the random int by 3 and assign its
    // remainder to a variable.
    int c_num = rand() % 3;

    // Assign a move to the computer's random number.
    char c_move;
    switch (c_num) {
        case 0:
            c_move = 'r';
            break;
        case 1:
            c_move = 'p';
            break;
        case 2:
            c_move = 's';
            break;
    }

    // Return the Computer's Move
    return c_move;
}

char get_user()
{
    using namespace std;

    // Get the user's move
    char move;
    cout << "Enter your move (Rock = r , Paper = p , Scissors = s):" << endl;
    cin >> move;
    cout << endl;

    // Return the chosen move to the main function
    return move;
}

int main()
{
    using namespace std;

    while (true) {
        // Get the user's move
        char user_move = get_user();

        // Get the computer's move
        char comp_move = get_comp();

        // Print the countdown dialogue
        countdown();

        cout << endl;

        // Declare a winner
        show_winner(user_move, comp_move);

        for (time_t t = time(0) + 1; time(0) < t;) {}

        /* Prompt the user to play another round.
         * Any inpput besides "yes", "Yes", "y", or "Y"
         * will break out of the main loop. */
        string again;
        cout << endl;
        cout << "Enter Y to Play Again" << endl;
        cin >> again;
        if (again == "Y") {}
        else break;
    }


    // Main Function Return
    return 0;
}


