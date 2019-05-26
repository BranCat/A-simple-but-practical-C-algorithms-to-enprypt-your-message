#include <iostream>
#include <iomanip>
#include <string>

using namespace std;

int main(){
    
    
    string alphabet {"abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ"};
    
    // Protection code corresponding to above letters 
    string key {"Q}E'TYUIOPASDFGHJKLMNBVZCXmnbvcxzasdfghjklqwertyupoi"};
       
    cout<<"\n";
    string secret_message {};
    cout<<"Enter your secret message: ";
    getline(cin,secret_message);
    
// ********* My code, it is working perfect. **********************//
    cout<<"Secret massage is: "<<secret_message<<endl;
    
    // Add a proection code
    for (int i{0}; i<secret_message.length();++i){
        for(int j{0};j<alphabet.length();++j){
            if(secret_message.at(i) == alphabet.at(j)){
                secret_message.at(i) = key.at(j);
                break;
            }
        }
    }
    
    cout<<"After coding proection, secret code is "<<secret_message<<endl;
    
    // Decipher process
    for(int i{0};i<secret_message.length();++i){
        for(int j{0};j<alphabet.length();++j){
            if(secret_message.at(i) == key.at(j)){
                secret_message.at(i) = alphabet.at(j);
                break;
            }
        }
    }
    
    cout<<"Original message is "<<secret_message<<endl;
    
        cout<<endl;
    return 0;
}
