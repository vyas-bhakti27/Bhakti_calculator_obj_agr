// calculator using object as an aguments

#include<iostream>
using namespace std;
class calculator{
    public:
          int input1;
          int input2;
          void setInput(int a,int b){
          input1=a;
          input2=b;
           }
           int add() {
           return input1+input2;
           }
           int sub() {
           return input1 - input2;
            }
            int mul() {
            return input1 * input2;
             }
             int div() {
            return input1 / input2;
             }
            int add(calculator obj1,calculator obj2) {
  
            return obj1.input1+ obj2.input2;
            }
            int sub(calculator obj1,calculator obj2) {
  
            return obj1.input1- obj2.input2;
            }
            int mul(calculator obj1,calculator obj2) {
  
            return obj1.input1 * obj2.input2;
            }
            int div(calculator obj1,calculator obj2) {
  
            return obj1.input1 / obj2.input2;
            }
};
int main(){

calculator obj1;
obj1.setInput(10,2);
cout << "The inputs:" << obj1.input1 <<" "<< obj1.input2<<endl;
cout <<"The sum of inputs is:"<< obj1.add();
cout <<"The subtraction of inputs is:"<< obj1.sub();
cout <<"The mutiplication of inputs is:"<< obj1.mul();
cout <<"The division of inputs is:"<< obj1.div();
return 0;
}
