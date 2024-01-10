#include <bits/stdc++.h>
using namespace std;
string s;
struct Game  //This is the information we will be storing about our game
{
    string name, description;
    double price;
};

map <string, Game> gameLibrary;

void add() //first funtion, this will add a new game to our list
{
    string n, d;
    double p;
    cout<<"Enter the name of the game you want to add: ";
    cin>>n;
    cout<<endl;
    cout<<"Enter the description of the game you are adding: "<<endl;
    getline(cin, d);
    cout<<endl;
    cout<<"Enter the price of the game: ";
    cin>>p;

    gameLibrary[n] = {n, d, p};
    cout<<n<<"has been added to the list.";
}

void rem()
{
    string n;
    cout<<"What game would you like to remove: "<<endl;
    getline(cin, n);

    gameLibrary.erase(n);
    cout<<n<<"has been erased."<<endl;
}

void library()
{
    for(map<string, Game>::iterator it = gameLibrary.begin(); it != gameLibrary.end(); ++it)
    {
        cout<< it->first << it->second <<endl;
    }
}
void help()
{
    cout<<"List of commands: add, rem, library, help"<<endl;
}

void ask()
{
    cout<<"What command would you like to perform: ";
    cin>>s;

    if(s == "add") add();
    else if(s == "rem") rem();
    else if(s == "library") library();
}


int main()
{
    cout<<"Welcome to your game library! Here you can keep information about all the games you own!"<<endl;
    cout<<"You can use commands: add, rem, library and help command to see this prompt again";
    ask();

    return 0;
}
