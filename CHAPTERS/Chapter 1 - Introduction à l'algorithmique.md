<!-- MarkDown for writing about the course -->

# Algorithls & Data Structures

## Plan de travail

1. Introduction

    * Overview

    * Why algorithms?

    * Resources

  
  
  
  
  
  

# Introduction

## Overview

What is **Algorithms & Data Structures**?
<ol>
<li>c'est un bloc d'instruction ou des commandes qui reçoit une entrée (input), il applique les modifications et les transformations nécessaires pour qu'il nous donne une sortie qui est la solution de notre problème!</li>
<li>méthode pour résoudre le problème.</li>
</ol>
What is **Data Structure**.
<ol>

<li>c'est une format special pour organiser, traiter, récupérer et stocker les données.</li>
<li>méthode pour stocker de l'information.</li>

</ol>

Why study **Algorithms**?
<p>
Leurs impact est très large et de grande portée.		
Exemples:
	- Web searching
	- Recommandations
	- social media feed
	- advertisements
	- video games
	- etc....
</p>
<p>
Les algorithmes dates à 2000 BC, avec l'apparition du feu, et les Hommes commence à développer des recettes*, etc...
Le pique de découverte des algos est dans les années 70s, et le dernier algorithm découvrit est l'algo do YOLO ("You Only Look Once") par Joseph Redmon en 2015.
</p>
<ul>
<li>Résoudre les problèmes!</li>
<li>Stimulation intellectuelle</li>
<li>Etre un bon programmeur</li>
<li>Voir la vie et l'univers d'une vision analytique, critique</li>
<li>Réussir les entretiens de stage ou d'emboche</li>
</ul>
<p>INVESTI DANS CETTE FORMATION!
investi dans les algorithmes et les structures de données.</p>

<ol>
<p>à faire:
<li>Installer JAVA sur vous PC!<br></li>
<li>Soit vous travailler avec Eclipse | IntelliJ | VS-code.<br></li>
IntelliJ: <a>https://youtu.be/Ope4icw6bVk</a><br>
Eclipse: <a>https://youtu.be/_7OM-cMYWbQ</a><br>
<li>JAVA concepts: Loops, functions, objects, recursion, arrays!</li>
</p>
</ol>


INPT is receiving new students for the year 2023/2024.
Student are given a paper holding a number from 1 to 10, and each student enter the institut in turn after he passes his paper to the student behind him, each student is requested to answer this question before entering: what is the total of the numbers written in the papers you are currently possessing?

Example: 
- array[1,2,3,4,5,6,7,8,9]
- answer: [1,3,6,10,15,21,28,36,45,55]

code:
```java
import java.util.ArrayList;
import java.util.Scanner;

public class test {

    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);
        
        int t = s.nextInt();
        
        ArrayList<Integer> test = new ArrayList<Integer>(t);
        
        for (int i = 0; i < t; i++) {
            int r = s.nextInt();
            test.add(r);
        }
        
        ArrayList<Integer> ans = new ArrayList<Integer>(t);
        
       
        int saver = 0;
        
        for (int j = 0; j < test.size(); j++) {
            saver += test.get(j);
            ans.add(saver);
        }
        
        System.out.println(ans);
        
        s.close();
    }
}
```