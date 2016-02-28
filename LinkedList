#include "MyLinkedList.cpp"
#include <iostream>

using namespace std;
int menu();

int main()
{
    MyLinkedList<int> testList;
    int number, choice;
    char letter;
    do
    {
        choice=menu();

        switch(choice)
        {
            case 1:     // Ask the user to enter an item
                        cout<<"Enter an item to the list"<<endl;
                        cin >> number;
                        testList.insertItem(number);

                        break;

            case 2:     // To delete a given item
                        cout<<"\nEnter a number to delete"<<endl;
                        int takeout;
                        cin>>takeout;
                        testList.deleteItem(takeout);
                        if (testList.deleteItem(takeout) == true)
                            cout<<"\nItem found, and it's deleted from the list"<<endl;
                        else
                            cout<<"\nItem is not in the list"<<endl;

                        break;

            case 3:     cout<<"\nEnter a number to search"<<endl;
                        int look;
                        cin>>look;
                        if(testList.searchItem(look) == true)
                            cout<<"\nItem found, and it's in the list"<<endl;

                        else
                            cout<<"\nThe item you're looking for is not in the list"<<endl;

                        break;

            case 4:     // To return the length of the list
                        cout<<"\nThe length of the list is " <<testList.getLength()<<endl;

                        break;

            case 5:     int occurences;
                        cout<<"\nEnter a number to delete all the occurences of an item"<<endl;
                        cin>>occurences;
                        testList.deleteOccurencesItem(occurences);

                        if (testList.deleteOccurencesItem(occurences) == true)
                            cout<<"\nItem(s) found, and it's deleted from the list"<<endl;
                        else
                            cout<<"\nItem(s) is not in the list"<<endl;

                        break;


            case 6:     //To return if the list is full
                    if(testList.isFull ()== true)
                         cout<<"\nThe list is full"<<endl;

                    else
                        cout<<"\nThe list is not full"<<endl;

                        break;


            case 7:     // To return if the list if empty or not
                    if(testList.isEmpty()== true)
                        cout<<"\nThe list is empty"<<endl;

                    else
                        cout<<"\nThe list is not empty"<<endl;

                        break;


            case 10:
                    cout<<"\n"<<testList.printInfo()<<endl;
                    break;
        }


        // Ask the user if he/she wants to enter more item
        cout<<"\nPress any letter to continue and n to end"<<endl;
        cin>>letter;

    }while(letter != 'n');






}

int menu()
{
    int x;

        cout<<"\nEnter 1 to insert"<<endl;
        cout<<"\nEnter 2 to delete"<<endl;
        cout<<"\nEnter 3 to search"<<endl;
        cout<<"\nEnter 4 to get length"<<endl;
        cout<<"\nEnter 5 to delete all occurences"<<endl;
        cout<<"\nEnter 6 to check if the list is full"<<endl;
        cout<<"\nEnter 7 to check if the list is empty"<<endl;
        cout<<"\nEnter 8 to make the list empty"<<endl;
        cout<<"\nEnter 9 to printing the list"<<endl;

        cin>>x;

    if (x<1 || x>9)
        cout<<"The number you enter is either too small or too large!"<<endl;

    else
        return x;

}

//#endif
