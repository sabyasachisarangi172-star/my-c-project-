# my-c-project-
this repository  has all my c++ codes with things like games basic calculator etc.
#include <iostream>
#include <string>

int main() {
    int choice = 0;
    int health = 50; // This is our main health tracker
    std::string name = "god";
    std::string wepon = "destroyer";

    // --- MENU LOOP ---
    do {
        std::cout << "\n=== MENU ===\n";
        std::cout << "wassup gamer !\n";
        std::cout << "1. set the warriors name\n";
        std::cout << "2. name of the destroyer\n";
        std::cout << "choose one of two: ";
        std::cout << "the hp of yours is " << health << "\n";
        std::cin >> choice;

        if (choice == 1) {
            std::cout << "okhie warrior set your name\n";
            std::cin >> name;
            std::cout << "good noon " << name << "\n";
        }
        else if (choice == 2) {
            std::cout << "okhie warrior lets set the warrior\n";
            std::cout << "3. fists\n4. ak47\n5. bombs\n6. mystic warrior\n";
            std::cin >> choice;
            if (choice == 3) std::cout << "well well be the bruce lee here\n";
            else if (choice == 4) std::cout << "aha!! though ya you would choose it..\n";
            else if (choice == 5) std::cout << "what !!!!!! we aint gonna destroy the village!!\n";
            else if (choice == 6) std::cout << "mystic paths chosen...\n";
            
            std::cout << "we are all set " << name << " lets goo\n";
            choice = 2; // Keep loop stable
        }
    } while (choice != 3 && choice != 10 && choice != 11 && choice != 12); 
    // Loop breaks when entering battle choices below

    std::cout << "\njumping into the terrain of death are you ready " << name << " \n";
    std::cout << "here the rules are simple: you dodge, you save life; you get hit, you lose points.\n";
    std::cout << "the weapon you chose will be the way to destroy your enemies!\n";
    std::cout << "5 questions = 5 boss levels. Choose your battlefield:\n";
    std::cout << "10. english the mind gamer\n";
    std::cout << "11. maths the ultimate eater\n";
    std::cout << "12. science the demon\n";
    std::cout << "Enter battlefield code: ";
    std::cin >> choice;

    // ================= ENGLISH BATTLEFIELD =================
    if (choice == 10) {
        std::cout << "\nwell you chose the mind gamer, here are the questions!\n";
        
        // Q1
        std::cout << "[Boss 1] Pick choice 13 to hit: ";
        std::cin >> choice;
        if (choice == 13) {
            std::cout << "correctt!!! moving on to the next level\n";
            health = health + 10;
        } else {
            std::cout << "idiot you lost life\n";
            health = health - 10;
        }

        // Q2
        std::cout << "\nhere is your next question warrior. Pick choice 18 to hit: ";
        std::cin >> choice;
        if (choice == 18) {
            std::cout << "correctt!!!\n";
            health = health + 10;
        } else {
            std::cout << "idiot you lost life\n";
            health = health - 10;
        }

        // Q3
        std::cout << "\nnext demon. Pick choice 27 to hit: ";
        std::cin >> choice;
        if (choice == 27) {
            std::cout << "correctt!!!\n";
            health = health + 10;
        } else {
            std::cout << "idiot you lost life\n";
            health = health - 10;
        }

        // Q4
        std::cout << "\nthe new piglin. Pick choice 31 to hit: ";
        std::cin >> choice;
        if (choice == 31) {
            std::cout << "correctt!!!\n";
            health = health + 10;
        } else {
            std::cout << "idiot you lost life\n";
            health = health - 10;
        }

        // Q5
        std::cout << "\nthe last and horrifying question. Pick choice 33 to hit: ";
        std::cin >> choice;
        if (choice == 33) {
            std::cout << "correctt!!!\n";
            health = health + 10;
        } else {
            std::cout << "idiot you lost life\n";
            health = health - 10;
        }

        std::cout << "\nthe war is over warrior\n";
        if (health <= 50) { // Fixed Operator =< to <=
            std::cout << "ehe ehe try harder " << name << " final health power: " << health << "\n";
        } else {
            std::cout << "well you survived level 1 congratulations !!!!! Final Health: " << health << "\n";
        }
    }

    // ================= MATHS BATTLEFIELD =================
    else if (choice == 11) {
        std::cout << "\nwell you chose the eater ... the hunger is on!\n";
        
        // Q1
        std::cout << "[Boss 1] Pick choice 41 to hit: ";
        std::cin >> choice;
        if (choice == 41) {
            std::cout << "correctt!!!\n";
            health = health + 10;
        } else {
            std::cout << "idiot you lost life\n";
            health = health - 10;
        }

        // Q2
        std::cout << "\nhere is your next question warrior. Pick choice 45 to hit: ";
        std::cin >> choice;
        if (choice == 45) {
            std::cout << "correctt!!!\n";
            health = health + 10;
        } else {
            std::cout << "idiot you lost life\n";
            health = health - 10;
        }

        // Q3
        std::cout << "\nnext demon. Pick choice 50 to hit: ";
        std::cin >> choice;
        if (choice == 50) { // Fixed typo check
            std::cout << "correctt!!!\n";
            health = health + 10;
        } else {
            std::cout << "idiot you lost life\n";
            health = health - 10;
        }

        // Q4
        std::cout << "\nthe new piglin. Pick choice 56 to hit: ";
        std::cin >> choice;
        if (choice == 56) {
            std::cout << "correctt!!!\n";
            health = health + 10;
        } else {
            std::cout << "idiot you lost life\n";
            health = health - 10;
        }

        // Q5
        std::cout << "\nthe last and horrifying question. Pick choice 61 to hit: ";
        std::cin >> choice;
        if (choice == 61) {
            std::cout << "correctt!!!\n";
            health = health + 10;
        } else {
            std::cout << "idiot you lost life\n";
            health = health - 10;
        }

        std::cout << "\nthe war is over warrior\n";
        if (health <= 50) {
            std::cout << "ehe ehe try harder " << name << " final health power: " << health << "\n";
        } else {
            std::cout << "well you survived level 1 congratulations !!!!! Final Health: " << health << "\n";
        }
    }

    // ================= SCIENCE BATTLEFIELD =================
    else if (choice == 12) {
        std::cout << "\nwell you chose the demon which invaded the physical world!\n";
        
        // Q1
        std::cout << "[Boss 1] Pick choice 62 to hit: ";
        std::cin >> choice;
        if (choice == 62) {
            std::cout << "correctt!!!\n";
            health = health + 10;
        } else {
            std::cout << "idiot you lost life\n";
            health = health - 10;
        }

        // Q2
        std::cout << "\nhere is your next question warrior. Pick choice 67 to hit: ";
        std::cin >> choice;
        if (choice == 67) {
            std::cout << "correctt!!!\n";
            health = health + 10;
        } else {
            std::cout << "idiot you lost life\n";
            health = health - 10;
        }

        // Q3
        std::cout << "\nnext demon. Pick choice 71 to hit: ";
        std::cin >> choice;
        if (choice == 71) {
            std::cout << "correctt!!!\n";
            health = health + 10;
        } else {
            std::cout << "idiot you lost life\n";
            health = health - 10;
        }

        // Q4
        std::cout << "\nthe new piglin. Pick choice 76 to hit: ";
        std::cin >> choice;
        if (choice == 76) {
            std::cout << "correctt!!!\n";
            health = health + 10;
        } else {
            std::cout << "idiot you lost life\n";
            health = health - 10;
        }

        // Q5
        std::cout << "\nthe last and horrifying question. Pick choice 81 to hit: ";
        std::cin >> choice;
        if (choice == 81) {
            std::cout << "correctt!!!\n";
            health = health + 10;
        } else {
            std::cout << "idiot you lost life\n";
            health = health - 10;
        }

        std::cout << "\nthe war is over warrior\n";
        if (health <= 50) {
            std::cout << "ehe ehe try harder " << name << " final health power: " << health << "\n";
        } else {
            std::cout << "well you survived level 1 congratulations !!!!! Final Health: " << health << "\n";
        }
    }

    return 0;
}
