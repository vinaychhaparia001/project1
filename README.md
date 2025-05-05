#  project1
#include<iostream.h>
#include<conio.h>
#include<stdio.h>
#include<string.h>
#include<fstream.h>

void cd(int coi);
void shci();

void writeoxy(int c,int r,char data[])
{
    gotoxy(c,r);
    cout<<data;
}
void clear()
{
   for (int r=7;r<=22;r++)
   {
       for (int c=2;c<=76;c++)
       {
	  gotoxy(c,r);
	  cout<<" ";
       }
   }
}
void clearci()
{
   for (int r=7;r<=23;r++)
   {
       for (int c=49;c<=78;c++)
       {
	  gotoxy(c,r);
	  cout<<" ";
       }
   }
}
void box()
{
    int row=1,col=1;
    char ch;
    gotoxy(1,1);
    ch=201;
    cout<<ch;
    for(col=2;col<=78;col++)
    {
	gotoxy(col,row);
	ch=205;
	cout<<ch;
    }
    gotoxy(79,1);
    ch=187;
    cout<<ch;
    for(row=2;row<=23;row++)
    {
	if(row!=6)
	{
	    gotoxy(col,row);
	    ch=186;
	    cout<<ch;
	}
	else
	{
	    gotoxy(col,row);
	    ch=185;
	    cout<<ch;
	}
    }
    gotoxy(79,24);
    ch=188;
    cout<<ch;
    row=24;
    for(col=78;col>=2;col--)
    {
	gotoxy(col,row);
	ch=205;
	cout<<ch;
    }
    gotoxy(1,24);
    ch=200;
    cout<<ch;
    col=1;
    for(row=23;row>=2;row--)
    {   if(row==6||row==4)
	{
	    gotoxy(col,row);
	    ch=204;
	    cout<<ch;
	}
	else
	{
	    gotoxy(col,row);
	    ch=186;
	    cout<<ch;
	}
    }
    for(col=2;col<=78;col++)
    {
	gotoxy(col,6);
	ch=205;
	cout<<ch;
    }
    for(col=2;col<=78;col++)
    {
	gotoxy(col,4);
	ch=205;
	cout<<ch;
    }
    gotoxy(16,2);
    cout<<"B H A R T I  C O M P U T E R   E D U C A T I O N ";
    gotoxy(18,3);
    cout<<"N A J A F G A R H , N E W  D E L H I : 110043";
}
void disp_box()
{   char ch;
    int col,row;
    for(row=2;row<=23;row++)
    {
	if(row==6||row==8)
	{
	    gotoxy(79,row);
	    ch=185;
	    cout<<ch;
	}
	else
	{
	    gotoxy(79,row);
	    ch=186;
	    cout<<ch;
	}
    }
    for(row=2;row<=23;row++)
    {
	if(row==6||row==8)
	{
	    gotoxy(1,row);
	    ch=204;
	    cout<<ch;
	}
	else
	{
	    gotoxy(1,row);
	    ch=186;
	    cout<<ch;
	}
    }
    for(row=7;row<=23;row++)
    {
	if(row==8)
	{
	    gotoxy(12,row);
	    ch=216;
	    cout<<ch;
	}
	else
	{
	    gotoxy(12,row);
	    ch=179;
	    cout<<ch;
	}
    }
    for(row=7;row<=23;row++)
    {
	if(row==8)
	{
	    gotoxy(40,row);
	    ch=216;
	    cout<<ch;
	}
	else
	{
	    gotoxy(40,row);
	    ch=179;
	    cout<<ch;
	}
    }
    for(row=7;row<=23;row++)
    {
	if(row==8)
	{
	    gotoxy(55,row);
	    ch=216;
	    cout<<ch;
	}
	else
	{
	    gotoxy(55,row);
	    ch=179;
	    cout<<ch;
	}
    }for(row=7;row<=23;row++)
    {
	if(row==8)
	{
	    gotoxy(67,row);
	    ch=216;
	    cout<<ch;
	}
	else
	{
	    gotoxy(67,row);
	    ch=179;
	    cout<<ch;
	}
    }
    for(col=2;col<=78;col++)
    {
	if(col==12||col==40||col==55||col==67)
	{
	    continue;
	}
	else
	{
	    gotoxy(col,8);
	    ch=205;
	    cout<<ch;
	}
    }
    for(col=2;col<=78;col++)
    {
	if(col==12||col==40||col==55||col==67)
	{
	    gotoxy(col,6);
	    ch=209;
	    cout<<ch;
	}
	else
	{
	    gotoxy(col,6);
	    ch=205;
	    cout<<ch;
	}
    }
    for(col=78;col>=2;col--)
    {
	if(col==12||col==40||col==55||col==67)
	{
	     gotoxy(col,24);
	     ch=207;
	     cout<<ch;
	}
	else
	{
	    gotoxy(col,row);
	    ch=205;
	    cout<<ch;
	}
    }
}
void ssbox()
{
    int c,r;
    char ch;
    gotoxy(40,6);
    ch=203;
    cout<<ch;
    r=8;
    for(c=1;c<=79;c++)
    {
	if(c==1)
	{
	     ch=204;
	     gotoxy(c,r);
	     cout<<ch;
	}
	else if(c==79)
	{
	     ch=185;
	     gotoxy(c,r);
	     cout<<ch;
	}
	else if(c==40)
	{
	    ch=206;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else
	{
	    ch=205;
	    gotoxy(c,r);
	    cout<<ch;
	}
    }
    c=40;
    for(r=7;r<=24;r++)
    {
	if(r==8)
	{
	    ch=206;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else if(r==24)
	{
	    ch=202;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else
	{
	    ch=186;
	    gotoxy(c,r);
	    cout<<ch;
	}
    }
}
void allsbox()
{
    int c,r;
    char ch;
    gotoxy(30,6);
    ch=203;
    cout<<ch;
    r=8;
    for(c=1;c<=79;c++)
    {
	if(c==1)
	{
	     ch=204;
	     gotoxy(c,r);
	     cout<<ch;
	}
	else if(c==79)
	{
	     ch=185;
	     gotoxy(c,r);
	     cout<<ch;
	}
	else if(c==30)
	{
	    ch=206;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else
	{
	    ch=205;
	    gotoxy(c,r);
	    cout<<ch;
	}
    }
    r=10;
    for(c=1;c<=79;c++)
    {
	if(c==1)
	{
	     ch=199;
	     gotoxy(c,r);
	     cout<<ch;
	}
	else if(c==79)
	{
	     ch=182;
	     gotoxy(c,r);
	     cout<<ch;
	}
	else if(c==30)
	{
	    ch=206;
	    gotoxy(c,r);
	    cout<<ch;
	}

	else
	{
	    ch=196;
	    gotoxy(c,r);
	    cout<<ch;
	}
    }
    c=30;
    for(r=7;r<=24;r++)
    {
	if(r==8)
	{
	    ch=206;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else if(r==24)
	{
	    ch=202;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else
	{
	    ch=186;
	    gotoxy(c,r);
	    cout<<ch;
	}
    }
    c=10;
    for(r=8;r<=24;r++)
    {
	if(r==8)
	{
	    ch=209;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else if(r==10)
	{
	    ch=197;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else if(r==24)
	{
	    ch=207;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else
	{
	    ch=179;
	    gotoxy(c,r);
	    cout<<ch;
	}
    }
    c=35;
    for(r=8;r<=24;r++)
    {
	if(r==8)
	{
	    ch=209;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else if(r==10)
	{
	    ch=197;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else if(r==24)
	{
	    ch=207;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else
	{
	    ch=179;
	    gotoxy(c,r);
	    cout<<ch;
	}
    }
    c=58;
    for(r=8;r<=24;r++)
    {
	if(r==8)
	{
	    ch=209;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else if(r==10)
	{
	    ch=197;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else if(r==24)
	{
	    ch=207;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else
	{
	    ch=179;
	    gotoxy(c,r);
	    cout<<ch;
	}
    }
    c=68;
    for(r=8;r<=24;r++)
    {
	if(r==8)
	{
	    ch=209;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else if(r==10)
	{
	    ch=197;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else if(r==24)
	{
	    ch=207;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else
	{
	    ch=179;
	    gotoxy(c,r);
	    cout<<ch;
	}
    }
}

class coursess
{
    private:
	int id;
	char cname[30],type[40],time[30],fee[20],content[50];
    public:
	void getcourse(int ci)
	{
	    id=ci;
	    writeoxy(20,7,"Courseid           :       ");
	    writeoxy(20,9,"Course Name        :       ");
	    writeoxy(20,11,"Course Type        :       ");
	    writeoxy(20,12,"(Certificate/Diploma/Crash)");
	    writeoxy(20,14,"Course durtion     :       ");
	    writeoxy(20,15,"(in Months)");
	    writeoxy(20,17,"Course fees        :    Rs.");
	    writeoxy(20,19,"Course Content     :       ");
	    gotoxy(49,7);
	    cout<<id;
	    gotoxy(49,9);
	    fflush(stdin);
	    gets(cname);
	    gotoxy(49,11);
	    fflush(stdin);
	    gets(type);
	    gotoxy(49,14);
	    fflush(stdin);
	    gets(time);
	    gotoxy(49,17);
	    fflush(stdin);
	    gets(fee);
	    gotoxy(49,19);
	    fflush(stdin);
	    gets(content);
	}
	void showcourse(int ro)
	{
	    writeoxy(2,7,"Courseid");
	    gotoxy(2,ro);
	    cout<<id;
	    writeoxy(20,7,"Course Name");
	    writeoxy(13,ro,cname);
	    writeoxy(41,7,"Course Type");
	    writeoxy(41,ro,type);
	    writeoxy(56,7,"Duration");
	    writeoxy(56,ro,time);
	    writeoxy(68,7,"Course Fees");
	    writeoxy(68,ro,fee);
	}
	void showcd()
	{
	    writeoxy(50,21,"COURSE ID:");
	    gotoxy(60,21);
	    cout<<id;
	    writeoxy(50,22,"COURSE   :");
	    writeoxy(60,22,cname);
	    writeoxy(50,23,"DURATION :");
	    writeoxy(60,23,time);
	}
	void sci(int r)
	{
	    writeoxy(50,8," ID ");
	    gotoxy(50,r);
	    cout<<id;
	    writeoxy(60,8,"COURSE NAME");
	    writeoxy(55,r,cname);
	}
	void show_s_course()
	{
	    writeoxy(50,7,"COURSE DETAILS");
	    writeoxy(41,10," Course id  :");
	    gotoxy(56,10);
	    cout<<id;
	    writeoxy(41,12," Course Name:");
	    writeoxy(56,12,cname);
	    writeoxy(41,14," Course Type:");
	    writeoxy(56,14,type);
	    writeoxy(41,16," Duration   :      months");
	    writeoxy(56,16,time);
	    writeoxy(41,18," Course Fees: Rs.");
	    writeoxy(58,18,fee);
	}
	void show_all_courses(int x)
	{
	    writeoxy(50,7,"COURSE DETAILS");
	    writeoxy(31,9," ID ");
	    gotoxy(31,x);
	    cout<<id;
	    writeoxy(45,9,"COURSE");
	    writeoxy(36,x,cname);
	    writeoxy(59,9,"DURATION");
	    gotoxy(59,x);
	    cout<<time<<"months";
	    writeoxy(71,9,"FEES");
	    gotoxy(69,x);
	    cout<<fee<<"Rs.";
	}
	int show_id()
	{
	    return id;
	}
}co;
class coid
{
    private:
	int id;
    public:
	void getid(int ci)
	{
	    id=ci+1;
	}
	void noid(int ci)
	{
	    id=ci-1;
	}
	int dispid()
	{
	    return id;
	}
}cid;

class temp
{
    private:
	int id;
	char cname[30],type[40],time[30],fee[20],content[50];
    public:
	void modifycourse(int ci)
	{
	    id=ci;
	    writeoxy(20,7,"Courseid           :       ");
	    writeoxy(20,9,"Course Name        :       ");
	    writeoxy(20,11,"Course Type        :       ");
	    writeoxy(20,12,"(Certificate/Diploma/Crash)");
	    writeoxy(20,14,"Course durtion     :       ");
	    writeoxy(20,15,"(in Months)");
	    writeoxy(20,17,"Course fees        :    Rs.");
	    writeoxy(20,19,"Course Content     :       ");
	    gotoxy(49,7);
	    cout<<id;
	    gotoxy(49,9);
	    fflush(stdin);
	    gets(cname);
	    gotoxy(49,11);
	    fflush(stdin);
	    gets(type);
	    gotoxy(49,14);
	    fflush(stdin);
	    gets(time);
	    gotoxy(49,17);
	    fflush(stdin);
	    gets(fee);
	    gotoxy(49,19);
	    fflush(stdin);
	    gets(content);
	}
}te;
class student
{
    private:
	char name[50],fname[40],add[80],cno[11];
	int rollno,ci;
    public:
	void getdata(int a)
	{
	    rollno=a;
	    writeoxy(2,8,"ROLL NO        :");
	    writeoxy(2,10,"student name   :");
	    writeoxy(2,12,"Father's name  :");
	    writeoxy(2,14,"mobile no.     :");
	    writeoxy(2,16," address       :");
	    writeoxy(2,17,"(Hno.,Landmark,City)");
	    writeoxy(2,19,"COURSE ID.     :");
	    gotoxy(20,8);
	    cout<<rollno;
	    gotoxy(20,10);
	    fflush(stdin);
	    gets(name);
	    gotoxy(20,12);
	    fflush(stdin);
	    gets(fname);
	    gotoxy(20,14);
	    fflush(stdin);
	    gets(cno);
	    gotoxy(20,16);
	    fflush(stdin);
	    gets(add);
	    clearci();
	    shci();
	    gotoxy(20,19);
	    cin>>ci;
	    clearci();
	    cd(ci);
	}

	void show_s_data()
	{
	    writeoxy(10,7,"Personal Details");
	    writeoxy(2,10," ROLLNO        :");
	    gotoxy(19,10);
	    cout<<rollno;
	    writeoxy(2,12," Name          :");
	    writeoxy(19,12,name);
	    writeoxy(2,14," FATHER's NAME :");
	    writeoxy(19,14,fname);
	    writeoxy(2,16," CONTACT       :");
	    writeoxy(19,16,cno);
	    writeoxy(2,18," ADDRESS:");
	    writeoxy(12,18,add);
	}
	void show_all_data(int x)
	{
	    writeoxy(10,7,"Personal Details");
	    writeoxy(2,9,"ROLL NO");
	    gotoxy(2,x);
	    cout<<rollno;
	    writeoxy(15,9,"NAME");
	    writeoxy(10,x,name);
	}
	int show_roll()
	{
	    return rollno;
	}
	int sshow_id()
	{
	    return ci;
	}
}stu;
class stemp
{
    private:
	char name[50],fname[40],add[80],cno[11];
	int rollno,ci;
    public:
	void modata(int a)
	{
	    rollno=a;
	    writeoxy(2,8,"ROLL NO        :");
	    writeoxy(2,10,"student name   :");
	    writeoxy(2,12,"Father's name  :");
	    writeoxy(2,14,"mobile no.     :");
	    writeoxy(2,16," address       :");
	    writeoxy(2,17,"(Hno.,Landmark,City)");
	    writeoxy(2,19,"COURSE ID.     :");
	    gotoxy(20,8);
	    cout<<rollno;
	    gotoxy(20,10);
	    fflush(stdin);
	    gets(name);
	    gotoxy(20,12);
	    fflush(stdin);
	    gets(fname);
	    gotoxy(20,14);

	    fflush(stdin);
	    gets(cno);
	    gotoxy(20,16);
	    fflush(stdin);
	    gets(add);
	    clearci();
	    shci();
	    gotoxy(20,19);
	    cin>>ci;
	    clearci();
	    cd(ci);
	}
}st;
class rollno
{
    private:
	int rno;
    public:
	void enter_roll(int r)
	{
	    rno=r+1;
	}
	void noroll(int r)
	{
	    rno=r-1;
	}
	int showroll()
	{
	    return rno;
	}
}rol;
void cbox()
{
    char ch;
    int r,c;
    r=20;
    for(c=49;c<=79;c++)
    {
	if(c==79)
	{
	    ch=182;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else if(c==60)
	{
	    ch=193;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else
	{
	    ch=196;
	    gotoxy(c,r);
	    cout<<ch;
	}
    }
    r=18;
    for(c=60;c<=79;c++)
    {
	if(c==79)
	{
	    ch=182;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else if(c==60)
	{
	    ch=218;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else
	{
	    ch=196;
	    gotoxy(c,r);
	    cout<<ch;
	}
    }
    c=49;
    for(r=20;r<=24;r++)
    {
	if(r==24)
	{
	    ch=207;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else if(r==20)
	{
	    ch=218;
	    gotoxy(c,r);
	    cout<<ch;
	 }
	else
	{
	    ch=179;
	    gotoxy(c,r);
	    cout<<ch;
	}
    }
    ch=179;
    gotoxy(60,19);
    cout<<ch;
}
void cibox()
{
    char ch;
    int r,c;
    r=7;
    for(c=49;c<=78;c++)
    {
	if(c==49)
	{
	    ch=218;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else if(c==54)
	{
	    ch=194;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else if(c==78)
	{
	    ch=191;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else
	{
	    ch=196;
	    gotoxy(c,r);
	    cout<<ch;
	}
    }
    r=9;
    for(c=49;c<=78;c++)
    {
	if(c==49)
	{
	    ch=218;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else if(c==54)
	{
	    ch=197;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else if(c==78)
	{
	    ch=180;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else
	{
	    ch=196;
	    gotoxy(c,r);
	    cout<<ch;
	}
    }
    r=23;
    for(c=49;c<=78;c++)
    {
	if(c==49)
	{
	    ch=192;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else if(c==54)
	{
	    ch=193;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else if(c==78)
	{
	    ch=217;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else
	{
	    ch=196;
	    gotoxy(c,r);
	    cout<<ch;
	}
    }
    c=49;
    for(r=8;r<=22;r++)
    {
	if(r==9)
	{
	    ch=195;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else
	{
	    ch=179;
	    gotoxy(c,r);
	    cout<<ch;
	}
    }
    c=78;
    for(r=8;r<=22;r++)
    {
	if(r==9)
	{
	    ch=180;
	    gotoxy(c,r);
	    cout<<ch;
	}
	else
	{
	    ch=179;
	    gotoxy(c,r);
	    cout<<ch;
	}
    }
    c=54;
    for(r=8;r<=22;r++)
    {
	if(r!=9)
	{
	    ch=179;
	    gotoxy(c,r);
	    cout<<ch;
	}
    }
}

void cd(int coi)
{
    fstream fin;
    int count=0;
    fin.open("vinay.dat",ios::in);
    fin.seekg(-1,ios::cur);
    int rec=fin.tellg()/sizeof(coursess);
    fin.seekg(0,ios::beg);
    for(int i=1;i<=rec;i++)
    {
	fin.read((char*)&co,sizeof(coursess));
	int cod=co.show_id();
	cbox();
	if(cod==coi)
	{
	    co.showcd();
	    count+=1;
	}
    }
    if(count<1)
    {
	writeoxy(50,22,"NO SUCH ID PRESENT");
	getch();
    }
    fin.close();
}

void shci()
{
    fstream fin;
    int count=10;
    fin.open("vinay.dat",ios::in);
    fin.seekg(-1,ios::cur);
    int rec=fin.tellg()/sizeof(coursess);
    fin.seekg(0,ios::beg);
    cibox();
    for(int i=1;i<=rec;i++)
    {
	fin.read((char*)&co,sizeof(coursess));
	co.sci(count);
	count++;
    }
    fin.close();
}
void showsrecord(int a)
{
    fstream fin,fout;
    int i,rec,check=0,idc;
    fout.open("student.dat",ios::in);
    fout.seekg(0,ios::end);
    rec=fout.tellg()/sizeof(student);
    fout.seekg(0,ios::beg);
    for(i=1;i<=rec;i++)
    {
	fout.read((char*)&stu,sizeof(student));
	if(a==stu.show_roll())
	{
	    stu.show_s_data();
	    check=1;
	    idc=stu.sshow_id();
	}
    }
    fout.close();
    if(check==0)
    {
	writeoxy(15,3,"NO RECORD FOUND");
	writeoxy(15,50,"NO RECORD FOUND");
    }
    fin.open("vinay.dat",ios::in);
    fin.seekg(0,ios::end);
    rec=fin.tellg()/sizeof(coursess);
    fin.seekg(0,ios::beg);
    for(i=1;i<=rec;i++)
    {
	fin.read((char*)&co,sizeof(coursess));
	if(idc==co.show_id())
	{
	    co.show_s_course();
	}
    }
    fin.close();
}
void show_all_records()
{
    fstream fin,fout;
    int i,rec,idc;
    fin.open("student.dat",ios::in);
    fin.seekg(0,ios::end);
    rec=fin.tellg()/sizeof(student);
    fin.seekg(0,ios::beg);
    int ro=11;
    for(i=1;i<=rec;i++)
    {
	fin.read((char*)&stu,sizeof(student));
	stu.show_all_data(ro);
	idc=stu.sshow_id();
	fout.open("vinay.dat",ios::in);
	fout.seekg(0,ios::end);
	int re=fout.tellg()/sizeof(coursess);
	fout.seekg(0,ios::beg);
	for(int j=1;j<=re;j++)
	{
	    fout.read((char*)&co,sizeof(coursess));
	    if(idc==co.show_id())
	    {
		co.show_all_courses(ro);
	    }
	}
	fout.close();
	ro++;
    }
    fin.close();
}
void main()
{
    clrscr();
    box();
    char  ch,choice,c;
    int coi,id;
    fstream fin,fout;
    do
    {
	clrscr();
	box();
	writeoxy(35,5,"MAIN MENU");
	writeoxy(27,9,"     ...W E L C O M E...");
	writeoxy(25,13,"1.-> C O U R S E  P O R T A L");
	writeoxy(25,15,"2.-> A D M I S S I O N  P O R T A L");
	writeoxy(25,17,"3.-> E X I T.");
	writeoxy(28,20,"PLEASE, ENTER YOUR CHOICE:-");
	choice=getche();
	if(choice=='1')
	{

	    clrscr();
	    box();
	    do
	    {
		writeoxy(35,5,"COURSE");
		writeoxy(30,8,"1.-> ADD COURSES");
		writeoxy(30,10,"2.-> SHOW COURSES");
		writeoxy(30,12,"3.-> MODIFY COURSES");
		writeoxy(30,14,"4.-> DELETE COURSES");
		writeoxy(30,16,"5.-> RETURN TO MAIN MENU");
		writeoxy(30,20,"PLEASE, ENTER YOUR CHOICE:-");
		ch=getche();
		clear();
		if(ch=='1')
		{
		    fin.open("vinay.dat",ios::in);
		    fin.seekg(0,ios::end);
		    int re=fin.tellg()/sizeof(coursess);
		    fin.seekg(0,ios::beg);
		    fin.close();
		    if(re==0)
		    {
			fin.open("courid.dat",ios::out);
			cid.getid(100);
			fin.write((char*)&cid,sizeof(coid));
			fin.close();
		    }
		    else
		    {
			fout.open("courid.dat",ios::in);
			fout.seekg(-1,ios::cur);
			int rec=fout.tellg()/sizeof(coid);
			fout.seekg(0,ios::beg);
			for(int j=1;j<=rec;j++)
			{
			    fout.read((char*)&cid,sizeof(coid));
			    coi=cid.dispid();
			}
			fout.close();
			fin.open("courid.dat",ios::app);
			cid.getid(coi);
			fin.write((char*)&cid,sizeof(coid));
			fin.close();
		    }
		    fin.open("courid.dat",ios::in);
		    fin.seekg(0,ios::end);
		    int rec=fin.tellg()/sizeof(coid);
		    fin.seekg(0,ios::beg);
		    int ci;
		    for(int i=1;i<=rec;i++)
		    {
			fin.read((char*)&cid,sizeof(coid));
			ci=cid.dispid();
		    }
		    fin.close();
		    fout.open("vinay.dat",ios::app);
		    co.getcourse(ci);
		    writeoxy(60,22,"Wanna save(y/n)?");
		    c=getche();
		    if(c=='y')
		    {
			fout.write((char*)&co,sizeof(coursess));
			fout.close();
		    }
		    else
		    {
			fout.close();
			fin.open("courid.dat",ios::app);
			cid.noid(ci);
			fin.write((char*)&cid,sizeof(coid));
			fin.close();
		    }
		    clrscr();
		    box();
		}
		else if(ch=='2')
		{
		    fin.open("vinay.dat",ios::in);
		    fin.seekg(0,ios::end);
		    int rec=fin.tellg()/sizeof(coursess);
		    fin.seekg(0,ios::beg);
		    int ro=9;
		    disp_box();
		    for(int i=1;i<=rec;i++)
		    {
			fin.read((char*)&co,sizeof(coursess));
			co.showcourse(ro);
			ro++;
		    }
		    getch();
		    fin.close();
		    clrscr();
		    box();
		}
		else if(ch=='3')
		{
		    int count=0;
		    gotoxy(25,10);
		    cout<<"ENTER ID YOU WANNA MODIFY:";
		    cin>>id;
		    clear();
		    fin.open("vinay.dat",ios::in);
		    fout.open("temp.dat",ios::out);
		    fin.seekg(-1,ios::cur);
		    int rec=fin.tellg()/sizeof(coursess);
		    fin.seekg(0,ios::beg);
		    for(int i=1;i<=rec;i++)
		    {
			fin.read((char*)&co,sizeof(coursess));
			int y=co.show_id();
			if(id==y)
			{
			    te.modifycourse(y);
			    writeoxy(60,22,"Wanna save(y/n)?");
			    c=getche();
			    if(c=='y')
			    {
				fout.write((char*)&te,sizeof(temp));
			    }
			    else
			    {
				fout.write((char*)&co,sizeof(temp));
			    }
			    count=1;
			}
			else
			{
			    fout.write((char*)&co,sizeof(temp));
			}
		    }
		    fin.close();
		    fout.close();
		    remove("vinay.dat");
		    rename("temp.dat","vinay.dat");
		    if(count==0)
		    {
			writeoxy(25,15,".....ROLL NO. NOT FOUND.....");
			getch();
		    }
		    clrscr();
		    box();
		}
		else if(ch=='4')
		{
		    writeoxy(35,5,"COURSE");
		    gotoxy(25,21);
		    cout<<"ENTER ID YOU WANNA DELETE:";
		    cin>>id;
		    clear();
		    fin.open("vinay.dat",ios::in);
		    fout.open("temp.dat",ios::out);
		    fin.seekg(0,ios::end);
		    int rec=fin.tellg()/sizeof(coursess);
		    fin.seekg(0,ios::beg);
		    int count=0;
		    for(int i=1;i<=rec;i++)
		    {
			fin.read((char*)&co,sizeof(coursess));
			int y=co.show_id();
			if(id!=y)
			{
			    fout.write((char*)&co,sizeof(temp));
			}
			else
			{
			    count+=1;
			}
		    }
		    fin.close();
		    fout.close();
		    if(count<1)
		    {
			writeoxy(25,12,"R  E C O R D  N O T  F O U N D");
			writeoxy(25,14,"    T R Y  A G A I N   ");
			getch();
		    }
		    else
		    {
			gotoxy(27,14);
			cout<<"....Record deleted....";
			getch();
		    }
		    remove("vinay.dat");
		    rename("temp.dat","vinay.dat");
		    clrscr();
		    box();
		}
		else if(ch=='5')
		{
		    break;
		}
		else
		{
		    writeoxy(35,5,"COURSE");
		    writeoxy(18,20,"..PLEASE ENTER VALID CHOICE..");
		    getch();
		    clrscr();
		    box();
		}
	    }while(ch!='5');

	}
	else if(choice=='2')
	{
	    clrscr();
	    box();
	    do
	    {
		writeoxy(35,5,"STUDENTS");
		writeoxy(25,8,"1.-> ADD STUDENT DETAILS");
		writeoxy(25,10,"2.-> SHOW STUDENT DETAILS");
		writeoxy(25,12,"3.-> MODIFY STUDENT DETAILS");
		writeoxy(25,14,"4.-> DELETE STUDENT's DETAILS");
		writeoxy(25,16,"5.-> RETURN TO MAIN MENU");
		writeoxy(25,18,"PLEASE ENTER YOUR CHOICE:");
		ch=getche();
		clear();
		if(ch=='1')
		{
		    int r;
		    fin.open("student.dat",ios::in);
		    fin.seekg(0,ios::end);
		    int re=fin.tellg()/sizeof(student);
		    fin.seekg(0,ios::beg);
		    fin.close();
		    if(re==0)
		    {
			fin.open("rolno.dat",ios::out);
			rol.enter_roll(0);
			fin.write((char*)&rol,sizeof(rollno));
			fin.close();
		    }
		    else
		    {
			fout.open("rolno.dat",ios::in);
			fout.read((char*)&rol,sizeof(rollno));
			r=rol.showroll();
			fout.close();
			fin.open("rolno.dat",ios::out);
			rol.enter_roll(r);
			fin.write((char*)&rol,sizeof(rollno));
			fin.close();
		    }
		    fin.open("rolno.dat",ios::in);
		    //fin.seekg(0,ios::end);
		    //int rec=fin.tellg()/sizeof(rollno);
		   // fin.seekg(0,ios::beg);
		   int ci;
		   // for(int i=1;i<=rec;i++)
		   // {
		   fin.read((char*)&rol,sizeof(rollno));
		   r=rol.showroll();
		   //}
		    fin.close();
		    fout.open("student.dat",ios::app);
		    stu.getdata(r);
		    writeoxy(62,19,"Wanna save(y/n)?");
		    c=getche();
		    if(c=='y')
		    {
			fout.write((char*)&stu,sizeof(student));
			fout.close();
		    }
		    else
		    {
			fout.close();
			fin.open("rolno.dat",ios::out);
			rol.noroll(r);
			fin.write((char*)&rol,sizeof(rollno));
			fin.close();
		    }
		    clrscr();
		    box();
		}
		else if(ch=='2')
		{
		    int rn;
		    clear();
		    writeoxy(30,11,"1.SINGLE STUDENT DETAILS");
		    writeoxy(30,13,"2.ALL STUDENT DETAILS");
		    c=getche();

		    if(c=='1')
		    {
			clear();
			writeoxy(30,15,"Enter rollno u wanna show:");
			cin>>rn;
			clear();
			showsrecord(rn);
			ssbox();
			getch();
		    }
		    else if(c=='2')
		    {
			clear();
			show_all_records();
			allsbox();
			getch();
		    }
		    else
		    {
			writeoxy(25,16,"DON'T HAVE SUCH CHOICE....");
			getch();
		    }
		    clrscr();
		    box();
		}
		else if(ch=='3')
		{
		    int rn,count=0;
		    gotoxy(25,12);
		    cout<<"Enter roll no u wanna modify:";
		    cin>>rn;
		    fin.open("student.dat",ios::in);
		    fout.open("stemp.dat",ios::out);
		    fin.seekg(-1,ios::cur);
		    int rec=fin.tellg()/sizeof(student);
		    fin.seekg(0,ios::beg);
		    if(rec==0)
		    {
			writeoxy(20,22,"NO RECORD PRESENT IN DATABASE..");
			getch();
		    }
		    else
		    {
			for(int i=1;i<=rec;i++)
			{
			    fin.read((char*)&stu,sizeof(student));
			    int y=stu.show_roll();
			    if(rn==y)
			    {
				st.modata(rn);
				writeoxy(62,19,"Wanna save(y/n)?");
				c=getche();
				if(c=='y')
				{
				    fout.write((char*)&st,sizeof(stemp));

				}
				else
				{
				    fout.write((char*)&st,sizeof(stemp));
				}
				count=1;
			    }
			    else
			    {
				fout.write((char*)&stu,sizeof(stemp));
			    }
			}
		    }
		    fin.close();
		    fout.close();
		    remove("student.dat");
		    rename("stemp.dat","student.dat");
		    if(count==0)
		    {
			writeoxy(25,15,".....ROLL NO. NOT FOUND.....");
			getch();
		    }
		    clrscr();
		    box();
		}
		else if(ch=='4')
		{
		    int rn;
		    gotoxy(25,10);
		    cout<<"ENTER ROLL NO. YOU WANNA DELETE:";
		    cin>>rn;
		    fin.open("student.dat",ios::in);
		    fout.open("stemp.dat",ios::out);
		    fin.seekg(0,ios::end);
		    int rec=fin.tellg()/sizeof(student);
		    fin.seekg(0,ios::beg);
		    int count=0;
		    for(int i=1;i<=rec;i++)
		    {
			fin.read((char*)&stu,sizeof(student));
			int y=stu.show_roll();
			if(rn!=y)
			{
			    fout.write((char*)&stu,sizeof(stemp));
			}
			else
			{
			    count+=1;
			}
		    }
		    fin.close();
		    fout.close();
		    if(count<1)
		    {
			writeoxy(25,14,"R  E C O R D  N O T  F O U N D");
			writeoxy(25,15,"    T R Y  A G A I N   ");
			getch();
		    }
		    else
		    {
			gotoxy(27,14);
			cout<<"....Record deleted....";
			getch();
		    }
		    remove("student.dat");
		    rename("stemp.dat","student.dat");
		    clrscr();
		    box();
		}
		else if(ch=='5')
		{
		    break;
		}
		else
		{
		    clrscr();
		    box();
		    gotoxy(25,10);
		    cout<<"....PLEASE ENTER VALID CHOICE....";
		    getch();
		    clrscr();
		    box();
		}
	    }while(ch!=5);
	}
	else if(choice=='3')
	{
	    clrscr();
	    box();
	    writeoxy(27,10,"....T H A N k  Y O U....");
	    getch();
	    break;
	}
	else
	{
	    writeoxy(20,21,".....ENTER VALID CHOICE.....");
	    getch();
	    clear();
	}
    }while(choice!='3');
}
