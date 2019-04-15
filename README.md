#include <iostream>
#include <string>
#include <iomanip>

using namespace std;

class bankAccount

{
  public:
  
    bankAccount(int, double, string);
    void setAccountNumber(int a)
    {
      a = AccountNumber;
    }
    int getAccountNumber()
    { 
      cin >> a ;
      return a;
    }
    void setName(string n)
    {
      Name = n;
    }
    string getName()
    {
      cin >> n;
      return n;
    }
    void setbalanace(double b)
    {
      balance = b;
    }
    double getbalance()
    {
      cin >> b;
      return b;
    }
    bool withdraw(double amount);
    bool deposit(double amount);
  
  
  
  protected:
   
    int AccountNumber;
    double balance;
    string Name;
};

class checkingAccount : public bankAccount{
  public:
  void setminBalance(double m)
  {
    minBalance = m;
  }
  double getminBalance
  {
    cin >> minBalance;
    return minBalance;
  }
  void serviceCharges(double)
  {
    if(minBalance > balance)
    cout << "Balance has fallen below minimum balance./n An insufficient balance fee of $25 will occur.">> endl;
    cout << "Current balance is " << (b - 25):
    else
    cout << "Current balance is "<< b;
  }
  getserviceCharges
  {
    return serviceCharges;
  }
  
  protected:
  double minBalance;
  double serviceCharges;
};

int main()
{
bankAccount bank;
checkingAccount check;

bank.setAccountNumber();

cout << "Enter account number :" << bank.getAccountNumber() << endl;

bank.setName();

cout << "Enter Name associated with account number:" << bank.getName() << endl;

bank.setbalanace();

cout<< "Enter current balance:" << bank.getbalance() << endl;

check.setminBalance(100);






return 0;
}
