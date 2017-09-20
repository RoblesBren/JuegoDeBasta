# JuegoDeBasta
#include <iostream>
#include<cstdlib>
#include<cstring>
#include<ctime>

using namespace std;


int main()
{

    int a=65, z=90, dato=0, sus[4], i=27,l,m;
    char letra;
    string pides[6]= {"Nombre","Apellido","Ciudad/Pais","Flor/Fruto","Animal","Cosa"};
    string nom[i],ap[i],ciud[i],florf[i],anm[i],cosa[i];
    char n[i],apel[i],c[i],f[i],an[i],co[i];
    int cont[6], punom, punape, punciudad, punflor,punanmi,puncosa,total;

    srand(time(0));
    letra=rand()%(a-z) +a;

    cout<<"TE TOCO LA LETRA: "<<letra<<endl;

    cout<<pides[0]<<" con la letra "<<letra<<":"<<endl;
    cin>>n;
    cout<<pides[1]<<" con la letra "<<letra<<":"<<endl;
    cin>>apel;
    cout<<pides[2]<<" con la letra "<<letra<<":"<<endl;
    cin>>c;
    cout<<pides[3]<<" con la letra "<<letra<<":"<<endl;
    cin>>f;
    cout<<pides[4]<<" con la letra "<<letra<<":"<<endl;
    cin>>an;
    cout<<pides[5]<<" con la letra "<<letra<<":"<<endl;
    cin>>co;

    cont[0]=strlen(n);
    cont[1]=strlen(apel);
    cont[2]=strlen(c);
    cont[3]=strlen(f);
    cont[4]=strlen(an);
    cont[5]=strlen(co);
    string nombre(n);
    string apellido(apel);
    string ciudad(c);
    string fruto(f);
    string animal(an);
    string cosass(co);

    if(n[0]!=letra||cont[0]<4||n==apel||n==c||n==f||n==an||n==co)
    {
        punom=0;
    }
    else
    {
        punom=100;
    }
    if(apel[0]!=letra||cont[1]<4||apel==n||apel==c||apel==f||apel==an||apel==co)
    {
        punape=0;
    }
    else
    {
        punape=100;
    }
    if(c[0]!=letra||cont[2]<4||c==n||c==apel||c==f||c==an||c==co)
    {
        punciudad=0;
    }
    else
    {
        punciudad=100;
    }

    if(f[0]!=letra||cont[3]<4||f==n||f==apel||f==c||f==an||f==co)
    {
        punflor=0;
    }

    else
    {
        punflor=100;
    }
    if(an[0]!=letra||cont[4]<4||an==n||an==apel||an==c||an==f||an==co)
    {
        punanmi=0;
    }
    else
    {
        punanmi=100;
    }
    if(co[0]!=letra||cont[5]<4||co==n||co==apel||co==c||co==f||co==an)
    {
        puncosa=0;
    }
    else
    {
        puncosa=100;
    }

cout<<n<<": "<<punom<<endl<<apel<<": "<<punape<<endl<<c<<": "<<punciudad<<endl<<f<<": "<<punflor<<endl<<an<<": "<<punanmi<<endl<<co<<": "<<puncosa<<endl;

}
