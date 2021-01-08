# prime-checker
Write a C++ code with a function named "is_prime" that takes a positive integer argument and returns as its value the integer 1 if the argument is prime and returns the integer 0 otherwise in the main function. Thus, for example,


#include <iostream>
using namespace std;

int is_prime(int a){

    int isPrime = 1;
    if(a<=1){
        return 0;
    }
    else{
        for(int i=2; i<a; i++){
            if(a%i==0){
                isPrime = 0;
                break;
            }
        }

    }
    return isPrime;
}

int main(){

    int x;
    cout << "Enter the number: ";
    cin >> x;
    cout << is_prime(x);

    return 0;
}
