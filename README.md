# task-1-guess-a-number
#include<iostream>
using namespace std;
int main(){
    int n;

    cout<<" Generating random nnumber from 1 to N  "<<endl;
    cout<<"enter max limit of number:"<<endl;
    cin>>n;
    int guess;
    
    int num=rand()%n;
    
    while(guess!=num){
        cout<<"enter guess:"<<endl;
        cin>>guess;
        if(guess>num){
        cout<<"the random number is smaller than the guessed number , please try again"<<endl;

        }else if(guess<num){
        cout<<"the random number is larger than the guessed number , please try again"<<endl;
        }
    }
    cout<<"bingo the guessed number is correct. You won, congratulations..."<<endl;
    
    return 0;

}
