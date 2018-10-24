# TIPUS DE LLENGUATGES

## Activitat

1. Realitza una recerca per Internet , per tal d'esbrinar quins són els llenguatges de programació que en aquest moment s'estan utilitzant més en el mercat.

![llenguatges](/img/2018.png)

2. Amplia els coneixements sobre tres llenguatges que triïs dels mencionats anteriorment i introdueix un exemple de codi.

**JAVA**

Java és un llenguatge de programació de propòsit general, concurrent, orientat a objectes, que va ser dissenyat específicament per tenir tan poques dependències d'implementació com fos possible. La seva intenció és permetre que els desenvolupadors d'aplicacions escriguin el programa una vegada i ho s'executin en qualsevol dispositiu (conegut en anglès com WORA, o "write onze, run anywhere"), el que vol dir que el codi que és executat en una plataforma no ha de ser reconstruït localment per córrer en una altra.

**EXEMPLE DE CODI:**

	public class HelloWorld {

        public static void main(String[] args) {
            // Prints "Hello, World" to the terminal window.
            System.out.println("Hello, World");
        }

	}

**C**

C és un llenguatge de programació originalment desenvolupat per Dennis Ritchie entre 1969 i 1972 en els Laboratoris Bell, 2 com a evolució de l'anterior llenguatge B, al seu torn basat en BCPL.

Igual que B, és un llenguatge orientat a la implementació de Sistemes operatius, concretament Unix. C és apreciat per l'eficiència del codi que produeix i és el llenguatge de programació més popular per crear programari de sistemes, encara que també s'utilitza per crear aplicacions.

Es tracta d'un llenguatge de tipus de dades estàtiques, feblement tipificat, de mig nivell, ja que disposa de les estructures típiques dels llenguatges d'alt nivell però, al seu torn, disposa de construccions del llenguatge que permeten un control a molt baix nivell . Els compiladors solen oferir extensions al llenguatge que possibiliten barrejar codi en assemblador amb codi C o accedeix

**EXEMPLE DE CODI:**

	#include <stdio.h>
	int main()
    {
       // printf() displays the string inside quotation
       printf("Hello, World!");
       return 0;
    }
    
**C++**

C \++ és un llenguatge de programació dissenyat el 1979 per Bjarne Stroustrup. La intenció de la seva creació va ser el estendre al llenguatge de programació C mecanismes que permeten la manipulació d'objectes. En aquest sentit, des del punt de vista dels llenguatges orientats a objectes, el C ++ és un llenguatge híbrid.

Posteriorment es van afegir facilitats de programació genèrica, que es van sumar als paradigmes de programació estructurada i programació orientada a objectes. Per això se sol dir que el C ++ és un llenguatge de programació multiparadigma.

Actualment hi ha un estàndard, anomenat ISO C ++, al qual s'han adherit la majoria dels fabricants de compiladors més moderns. Existeixen també alguns intèrprets, com ara ROOT.

Una particularitat del C ++ és la possibilitat de redefinir els operadors, i de poder crear nous tipus que es comportin com tipus fonamentals.

**EXEMPLE DE CODI:**

    #include <iostream>
    using namespace std;

    int main() 
    {
        cout << "Hello, World!";
        return 0;
    }

3. Busca llenguatges de programació del següent tipus:
	* Llenguatges orientats a servidors.
	* Llenguatges orientats a objectes.
