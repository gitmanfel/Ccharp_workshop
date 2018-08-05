# Ccharp_workshop

Dans ce Workshop, nous allons découvrir ce qu'est le C#, son histoire et son rapport avec le framework .NET. 

# Qu'est-ce que le C# ?

Le C# est un langage de programmation créé par Microsoft en 2002.

Le C# est un langage dont la syntaxe ressemble un peu au C++ ou au Java qui sont d’autres langages de programmation très populaires. Le C# est le langage phare de Microsoft. Il fait partie d’un ensemble plus important. Il est en fait une brique de ce qu’on appelle le « Framework .NET ». 
Gardons encore un peu de suspens sur ce qu'est le framework .NET, nous découvrirons ce que c'est un peu plus loin dans le tutoriel.

Pour obtenir du binaire à partir d'un code écrit en C ou C++, on doit effectuer ce qu'on appelle une compilation. Le compilateur est un programme qui traduit le code source en binaire exécutable 

J'ai commencé à vous parler du C# qui était une brique du framework .NET. Il est temps d'en savoir un peu plus sur ce fameux framework.

Commençons par le commencement : comment cela se prononce ?

Citation : Shakespeare

DOTTE NETTE

Citation : maitre Capello

POINT NETTE

Je vous accorde que le nom est bizarre, point trop net pourrions-nous dire …
Surtout que le nom peut être trompeur. Avec l’omniprésence d’internet, son abréviation (net) ou encore des noms de domaines (.net), on pourrait penser que le framework .NET est un truc dédié à internet. Que nenni.

Pour simplifier, on peut dire qu’un framework est une espèce de grosse boite à fonctionnalités qui va nous permettre de réaliser des applications informatiques de toutes sortes.

Le framework .NET est un framework créé par Microsoft en 2002, en même temps que le C#, qui est principalement dédié à la réalisation d’applications fonctionnant dans des environnements Microsoft. Nous pourrons par exemple réaliser des programmes qui fonctionnent sous Windows, ou bien des sites web ou encore des applications qui fonctionnent sur téléphone mobile, etc.


# En résumé
Le C# est un langage de programmation permettant d’utiliser le framework .NET. C’est le langage phare de Microsoft.

Le framework .NET est une énorme boîte à fonctionnalités permettant la création d’applications.

Le C# permet de développer des applications de toutes sortes, exécutables par le CLR qui traduit le MSIL en binaire.

Il est possible de créer des assemblys de deux sortes : des assemblys de processus exécutables par le CLR et des assemblys de bibliothèques.


# La syntaxe générale du C#

Les lignes de code écrites avec le langage de développement C# doivent s’écrire dans des fichiers dont l’extension est .cs

Console.WriteLine("…");  est une instruction dédiée à l’affichage sur la console. 

# Attention chaque ligne de code doit être correcte syntaxiquement sinon le compilateur ne saura pas le traduire en langage exécutable.

Par exemple, si à la fin de mon instruction, je retire le point-virgule ou si j’orthographie mal le mot WriteLine, j’aurai :

https://openclassrooms.com/fr/courses/1526901-apprenez-a-developper-en-c/1527334-la-syntaxe-generale-du-c#/id/r-2774798

# Le caractère de terminaison de ligne
En général, une instruction en code C# s’écrit sur une ligne et se termine par un point-virgule. 
Ainsi, l’instruction que nous avons vue plus haut :

# Console.WriteLine("Hello World !!");

se termine au niveau du point-virgule.
Il aurait été possible de remplacer le code écrit :

class Program
{
    static void Main(string[] args)
    {
        Console.WriteLine("Hello World !!");
    }
}

par :

class Program {static void Main(string[] args) {Console.WriteLine("Hello World !!");}}

ou encore :

class Program
{
static void Main(string[] args)
    {
        Console
                
                
.WriteLine("Hello World !!"
                
            );
    }
}

# En général, pour que le code soit le plus lisible possible, on écrit une instruction par ligne et on indente le code de façon à ce que les blocs soient lisibles.


# En résumé
# Le code C# est composé d’une suite d’instructions qui se terminent par un point virgule.

# La syntaxe d’un code C# doit être correcte sinon nous aurons des erreurs de compilation.

# Il est possible de commenter son code grâce aux caractères « // », « /* » et « */ ».

# Visual Studio Express dispose d’un outil puissant qui permet d’aider à compléter ses instructions : la complétion automatique.



# Pratique

using System;
					
public class Program
{
	public static void Main()
	{
		Console.WriteLine("Hello World");
		
		string phrase = "Mon prénom est \"Félicien\"";
		
		
		
	string civilite = "M.";
		
		
Console.WriteLine(phrase);
		
		int age1 = 20;
int age2 = 30;
int moyenne = (age1 + age2) / 2;
		
		string codePostal = "5000";
string ville = "Namur";
string adresse = codePostal + " " + ville;
		
		Console.WriteLine(adresse); // affiche : 5000 Namur
		
		string[] jours = new string[7];
jours[0] = "Lundi";
jours[1] = "Mardi";
jours[2] = "Mercredi";
jours[3] = "Jeudi";
jours[4] = "Vendredi";
jours[5] = "Samedi";
jours[6] = "Dimanche";
		
		for (int i = 0; i < jours.Length; i++)
{
    Console.WriteLine(jours[i]);
}
	

		
		int age = 20;
age = age + 10; // age contient 30 (addition)
age++; // age contient 31 (incrémentation de 1)
age--; // age contient 30 (décrémentation de 1)
age += 10; // équivalent à age = age + 10 (age contient 40)
age /= 2; // équivalent à age = age / 2 => (age contient 20)
		
		Console.WriteLine("Choses à faire :");
Console.WriteLine("\t - Arroser les plantes");
Console.WriteLine("\t - connaitre c sharp");
		
		
		decimal compteEnBanque = 300;
bool estCrediteur = (compteEnBanque >= 0);
if (estCrediteur)
    Console.WriteLine("Votre compte est créditeur");

		
		if (compteEnBanque >= 0)
{
    Console.WriteLine("Voici comment ouvrir un livret …");
}
else
{
    Console.WriteLine("Votre compte est débiteur");
    Console.WriteLine("N’oubliez pas que les frais de découverts sont de …");
}
	
bool estAgeDe30Ans = age == 30;
Console.WriteLine(estAgeDe30Ans); // affiche True
		
bool estSuperieurA10 = age > 10;
Console.WriteLine(estSuperieurA10); // affiche True
		
bool estDifferentDe30 = age != 30;
Console.WriteLine(estDifferentDe30); // affiche False
		
		bool estVrai = true;
if (estVrai)
    Console.WriteLine("C'est vrai !");
else
    Console.WriteLine("C'est faux !");
		
		string login = "Nicolas";
string motDePasse = "test";
if (login == "Nicolas" && motDePasse == "test")
    Console.WriteLine("Bienvenue Nicolas");
else
    Console.WriteLine("Login incorrect");
		
		
		
	if (civilite == "Mlle")
    Console.WriteLine("Vous êtes une femme");
else if (civilite == "Mlle")
    Console.WriteLine("Vous êtes une femme non mariée");
else if (civilite == "M.")
    Console.WriteLine("Vous êtes un homme");
else
    Console.WriteLine("Je n'ai pas pu déterminer votre civilité");
	
	string sexe = "M.";
switch (sexe)
{
    case "M." :
        Console.WriteLine("Bonjour monsieur");
        break;
    case "Mme":
        Console.WriteLine("Bonjour madame");
        break;
    case "Mlle":
        Console.WriteLine("Bonjour mademoiselle");	
	
	    break;
	

	
}
		
	}
}

# Pour aller plus loin : https://openclassrooms.com/fr/courses/1526901-apprenez-a-developper-en-c

# //https://dotnetfiddle.net/dDegEZ (compilateur dans un moteur de recherche)

# https://stackify.com/java-vs-net-comparison/



