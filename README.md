# TIPUS DE LLENGUATGES

## Activitat

1. Realitza una recerca per Internet , per tal d'esbrinar quins són els llenguatges de programació que en aquest moment s'estan utilitzant més en el mercat.

![llenguatges](/img/2018.png)

[Link pagina web lleinguatges](https://www.tiobe.com/tiobe-index/)

2. Amplia els coneixements sobre tres llenguatges que triïs dels mencionats anteriorment i introdueix un exemple de codi.

**JAVA**

Java és un llenguatge de programació de propòsit general, concurrent, orientat a objectes, que va ser dissenyat específicament per tenir tan poques dependències d'implementació com fos possible. La seva intenció és permetre que els desenvolupadors d'aplicacions escriguin el programa una vegada i ho s'executin en qualsevol dispositiu (conegut en anglès com WORA, o "write onze, run anywhere"), el que vol dir que el codi que és executat en una plataforma no ha de ser reconstruït localment per córrer en una altra.

**EXEMPLE DE CODI:**

	public class Deposito {    

        //Campos de la clase
        private float diametro;
        private float altura;
        private String idDeposito;

        //Constructor sin parámetros auxiliar
        public Deposito () { //Lo que hace es llamar al constructor con parámetros pasándole valores vacíos
            this(0,0,"");            } //Cierre del constructor


        //Constructor de la clase que pide los parámetros necesarios
        public Deposito (float valor_diametro, float valor_altura, String valor_idDeposito) {
            if (valor_diametro > 0 && valor_altura > 0) {            
                diametro = valor_diametro;
                altura = valor_altura;
                idDeposito = valor_idDeposito;
            } else {
                diametro = 10;
                altura = 5;
                idDeposito = "000";
                System.out.println ("Creado depósito con valores por defecto diametro 10 metros altura 5 metros id 000" );
            }   } //Cierre del constructor

        public void setValoresDeposito (String valor_idDeposito, float valor_diametro, float valor_altura) {
            idDeposito = valor_idDeposito;
            diametro = valor_diametro;
            altura = valor_altura;
            if (idDeposito !="" && valor_diametro > 0 && valor_altura > 0) {
            } else {
                System.out.println ("Valores no admisibles. No se han establecido valores para el depósito");
                //Deposito (0.0f, 0.0f, ""); Esto no es posible. Un constructor no es un método y por tanto no podemos llamarlo
                idDeposito = "";
                diametro = 0;
                altura = 0;
            }     } //Cierre del método

        public float getDiametro () { return diametro; } //Método de acceso
        public float getAltura () { return altura; } //Método de acceso
        public String getIdDeposito () { return idDeposito; } //Método de acceso
        public float valorCapacidad () { //Método tipo función
            float capacidad;
            float pi = 3.1416f; //Si no incluimos la f el compilador considera que 3.1416 es double
            capacidad = pi * (diametro/2) * (diametro/2) * altura;
            return capacidad;
        }    

    } //Cierre de la clase

**C**

C és un llenguatge de programació originalment desenvolupat per Dennis Ritchie entre 1969 i 1972 en els Laboratoris Bell, 2 com a evolució de l'anterior llenguatge B, al seu torn basat en BCPL.

Igual que B, és un llenguatge orientat a la implementació de Sistemes operatius, concretament Unix. C és apreciat per l'eficiència del codi que produeix i és el llenguatge de programació més popular per crear programari de sistemes, encara que també s'utilitza per crear aplicacions.

Es tracta d'un llenguatge de tipus de dades estàtiques, feblement tipificat, de mig nivell, ja que disposa de les estructures típiques dels llenguatges d'alt nivell però, al seu torn, disposa de construccions del llenguatge que permeten un control a molt baix nivell . Els compiladors solen oferir extensions al llenguatge que possibiliten barrejar codi en assemblador amb codi C o accedeix

**EXEMPLE DE CODI:**

	/* ejemplo 14.- Lee una palabra y lo escribe al revés */

    #include <stdio.h>

    int main () {
    char l, palabra[21];
    int i;

    printf("Teclee una palabra de menos de 20 letras:");
    scanf("%s", palabra);

    i = 0;

    while(palabra[i++] != ‘\0') ;
        l = i-1; printf("%s tiene %d letras\n", palabra, l);

    printf("%s escrita al revés es: ", palabra);
    i = l;

    while (i > 0)
        printf("%c", palabra[--i]);
    return 0;

    }
    
**PYTHON**

Python és un llenguatge de programació interpretat que la seva filosofia fa èmfasi en una sintaxi que afavoreix un codi llegible.

Es tracta d'un llenguatge de programació multiparadigma, ja que suporta orientació a objectes, programació imperativa i, en menor mesura, programació funcional. És un llenguatge interpretat, usat tipat dinàmic i és multiplataforma.

És administrat per la Fundació per al programari de Python. Posseeix una llicència de codi obert, denominada Llicència Python Software Foundation, que és compatible amb la Llicència pública general de GNU

**EXEMPLE DE CODI:**

    #! /usr/bin/env python
    # -*- coding: utf-8 -*-

    def inversa (cadena):
        invertida = ""
        cont = len(cadena)
        indice = -1
        while cont >= 1:
            invertida += cadena[indice]
            indice = indice + (-1)
            cont -= 1
        return invertida

    def es_palindromo (cadena):
        palabra_invertida = inversa (cadena)
        indice = 0
        cont = 0
        for i in range (len(cadena)):
            if palabra_invertida[indice] == cadena[indice]:
                indice += 1
                cont += 1
            else:
                print "No es palindromo"
                break

        if cont == len(cadena): #Si el contador = a la cantidad de letras de la cadena
            print "Es palindromo" # es porque recorrió todo el ciclo for y todas las
                                                # letras son iguales

3. Busca llenguatges de programació del següent tipus:

	* Llenguatges orientats a servidors.
		* ASP.NET
        ASP.NET és un entorn per a aplicacions web desenvolupat i comercialitzat per Microsoft. És usat per programadors i dissenyadors per construir llocs web dinàmics, aplicacions web i serveis web XML. Va aparèixer el gener de 2002 amb la versió 1.0 del .NET Framework, i és la tecnologia successora de la tecnologia Active Server Pages (ASP). ASP.NET està construït sobre el Common Language Runtime, permetent als programadors escriure codi ASP.NET utilitzant qualsevol idioma admès per .NET Framework.

		* PERL
        Perl és un llenguatge de programació dissenyat per Larry Wall en 1987. Perl pren característiques del llenguatge C, del llenguatge interpretat bourne shell (sh), AWK, sed, Lisp i, en un grau inferior, de molts altres programes d'idiomes.

        Estructuralmente, Perl està basat en un estil de blocs com els del C o AWK, i va ser àmpliament adoptat per la seva destresa en el processament de text i no tenint cap de les limitacions dels altres llenguatges de script.

		* PHP
        PHP, acròim recursivo en anglès de PHP Personal Hypertext processador (preprocesador d'hipertext), és un llenguatge de programació de propòsit general de codi del costat del servidor originalment dissenyat per al desenvolupament web de contingut dinàmic

		* JSP
        JavaServer Pages (JSP) és una tecnologia que ajuda els desenvolupadors de programari a crear pàgines web dinàmiques basades en HTML i XML, entre altres tipus de documents. JSP és similar a PHP, però usa el llenguatge de programació Java.

        Per desplegar i executar pàgines JavaServer, es requereix un servidor web compatible amb contenidors servlet com Apache Tomcat o Jetty.

		* Visual Basic Sript
		
	* Llenguatges orientats a objectes.
		* ABAP
        ABAP (Advanced Business Application Programming) és un llenguatge de quarta generació, propietat de SAP, que es fa servir per programar la majoria dels seus productes (R / 3, mySAP Business suite ...). Utilitza sentències d'Open SQL per connectar-se amb pràcticament qualsevol base de dades. Compta amb milers de funcions per al maneig d'arxius, bases de dades, dates, etc. Permet connexions RFC (crides de funcions remotes) per connectar-se als sistemes SAP amb qualsevol altre sistema o programa de programació.

		* ActionScript
        Adobe ActionScript (fecha de lanzamiento en 1997) es el lenguaje de programación de la plataforma Adobe Flash. Originalmente desarrollado como una forma para que los desarrolladores programen de forma más interactiva. La programación con ActionScript permite mucha más eficiencia en las aplicaciones de la plataforma Flash para construir animaciones de todo tipo, desde simples a complejas, ricas en datos e interfaces interactivas. 

        * C Sharp (C#)
        C # (pronounced si sharp in English) és un llenguatge de programació orientat a objectes desenvolupat i estandarditzat per Microsoft com a part de la seva plataforma .NET, que després va ser aprovat com un estàndard per la ECMA (ECMA-334) i ISO (ISO / IEC 23270). C # és un dels llenguatges de programació dissenyats per a la infraestructura de llenguatge comú.

        La seva sintaxis bàsica deriva de C / C + + i utilitza el model d'objectes de la plataforma. NET, similar al de Java, encara que inclou millores derivades d'altres idiomes.

        * Clarion
        Clarion és un llenguatge ARAD (Advanced Rapid Application Development) a més de ser un entorn de desenvolupament integrat de Softvelocity [1] orientat a la programació d'aplicacions de bases de dades. És compatible amb una gran quantitat de bases de dades, incloses totes les de format SQL, ADO i XML, a més, pot generar sortides a HTML, XML, arxius de text i PDF entre d'altres. La última versió de Clarion disponible a la data (2016) és Clarion 10. També existeix la versió Clarion.NET, però després de diversos anys de desenvolupament encara està en versió beta i incompleta.

        * Clipper
        * D
        * Object Pascal
        * Gambas
        * GObject
        * Genie
        * Harbour
        * Eiffel
        * Fortran 90/95
        * Java
        * JavaScript
        * Lexico
        * Objective-C
        * Ocaml
        * Oz
        * R
        * Pascal
        * Perl
        * PHP
        * PowerScript
        * Processing
        * Python
        * Ruby
        * Self
        * Smalltalk
        * Swift
        * Magik
        * Vala
        * VB.NET
        * Visual FoxPro
        * Visual Basic 6.0
        * Visual DataFlex
        * Visual Objects
        * XBase++
        * DRP
        * Scala


