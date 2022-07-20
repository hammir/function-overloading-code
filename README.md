//function-overloading-code
#include <iostream>

/* run this program using the console pauser or add your own getch, system("pause") or input loop */
using namespace std;
double area_circle(double radius)
{
	cout<<"area of given circle is= "<<3.141592653589793238*(radius*radius)<<"sq.units";
}
double area_triangle(double base,double height)
{
	cout<<"area of given triangle is= "<<(base*height)/2<<"sq.units";
}
double area_rectangle(double length,double width)
{
	cout<<"area of given rectangle is= "<<length*width<<"sq.units";
}
int main() {
	double radius,base,height,length,width;
	int shape;
	cout<<"Choose the shape :\n1.Circle\n2.Triangle\n3.Rectangle ";
	cout<<"\n";
	cin>>shape;
	if(shape==1){
		cout<<"Enter radius of circle= ";
		cin>>radius;
		area_circle(radius);
	
		}
		
		else if(shape==2)
		{
			cout<<"\nEnter sides of triangle= ";
	cout<<"\n";
	cin>>base;
	cout<<"\n";
	cin>>height;
	cout<<"\n";
	area_triangle(base,height);
		}
	 else if(shape==3){
		cout<<"Enter sides of rectangle= ";
cout<<"\n";
cin>>length;
cout<<"\n";
cin>>width;
area_rectangle(length,width);
	}
	else{
		cout<<"invalid choice";
	}
	
	return 0;
}
