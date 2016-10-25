#include <iostream>
using namespace std;


class SodaCan{
	private:
		string my_brand;
		int my_Size;
		int my_Contents;
	
	public:
		
		SodaCan()
		{
			my_Brand=" ";
			my_Size=0;
			my_Contents=0;
		}
		SodaCan(string brand,int size,int contents)
		{
			my_Brand = brand;
			my_Size = size;
			my_Contents=contents;
		}
		bool isempty()
		{
			
		}
		void pourInSoda(int amount)
		{
			if (my_Contents==0)
			{
				return false;
			}
			else
			{
				return true;
			}
		}
		void drink(int amount)
		{
			my_Content -=amount;
		}
		void setSize(int size)
		{
			my_Size=size;
		}
		int getSize ()
		{
			return my_Size;
		}
		string getBrand()
		{
			return my_Brand;
		}
		void setBrand(string brand)
		{
			my_Brand=brand;
		}
		int getcontent()
		{
			return my_Contents;
		}
		
		
	
};

int main()
{
	string brand;
	int size;
	int contents;
	int choice;
	
	cout<<"\twelcome to Miyabi's Vending Machine!"<<endl;
	cout<<"what do you want to buy "<<endl;
	cout<<"1. buy a soda "<<"2. quit ";
	if(choice==1)
	{
		cout<<"pick the brand "<<endl;
		cin>>brand;
		can.setBrand(brand);
		cout<<"how many soda you want to buy "<<endl;
		cin>>contents;
		can.pourInSoda(contents)
		cout<<"choose the size "<<endl;
		cout<<"1.small"<<" "<<"2.medium"<<" "<<"3.large";
		cin>>size;
		can.setSize(size);
		
		cout<<"you just bought "<<can.getBrand()<<endl;
		cout<<"the amount you bought is "<<can.getcontent()<<endl;
		cout<<"the size you choose "<<can.getSize()<<endl;
		if(size==1)
		{
			cout<<"you choose small cup ";
		}
		else if(size==2)
		{
			cout<<"you choose medium cup ";
		}
		else if(size==3)
		{
			cout<<"you choose large cup ";
		}
		
	}
	/*cout<<"Please place your order! your wish is my command!"<<endl;
	cout<<"oh yeah ........... don't put any spaces in the brand name,ok!"<<endl;
	cout<<"gimme a brand size content"<<endl;
	cin>>brand>>size>>contents;*/
	
	SodaCan can;
	can.setBrand(brand);
	can.setSize(size);
	can.pourInSoda(contents);
	
	cout<<"Here you go: ";
	cout<<can.getcontent()<<"ounces of "<<can.getBrand()<<endl;
	return 0;
	}

# 3-problem-set-A-Soda-can
