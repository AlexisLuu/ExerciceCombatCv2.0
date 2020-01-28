#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int
main ()
{
  srand (time (NULL));
  int pv_heros = 100;
  int pv_monstre = 100;
  int choix = 0;
  int choix_monstre = 0;
  int pm_heros = 2;
  int pm_monstre = 2;
  int feu_monstre = 0;
  int poison_heros = 0;
  printf ("Heros : %d PV \n", pv_heros);
  printf ("Monstre : %d PV \n", pv_monstre);
  printf ("Heros : %d PM \n", pm_heros);
  printf ("Monstre : %d PM \n", pm_monstre);
  while (pv_monstre > 0 && pv_heros > 0)
        {
		printf ("Fangald le mage se prépare au combat !");
        printf (" Que faire ? \n (1) Attaquer \n (2) Se defendre \n");
        if (pm_heros >= 3)
    	{
    	   printf ("(3) Embraser l'adversaire \n");
    	}
    	if (pm_heros >= 5)
    	{
    	    printf ("(4) Utiliser un antidote \n");
    	}
        scanf ("%d", &choix);
        choix_monstre = rand () % 2 + 1;
        if (pm_monstre >=5 && feu_monstre == 1)
        {
             choix_monstre = rand () % 4 + 1;
        }
        if (pm_monstre >= 3)
        {
    	    choix_monstre = rand () % 3 + 1;
    	    if (poison_heros == 1)
            {
    	        choix_monstre = rand () % 2 + 1;
            }
    	}
    
        if (choix == 1)
    	{
    	    if (choix_monstre == 1)
    	    {
    	        printf ("Heros attaque Monstre, Monstre perd 20 PV ! \n");
    	        pv_monstre = pv_monstre - 20;
    	        printf ("Monstre contre-attaque ! Heros perd 16 PV ! \n");
    	        pv_heros = pv_heros - 16;
    	        printf ("Heros : %d PV \n", pv_heros);
    	        printf ("Monstre : %d PV \n", pv_monstre);
             }
             
        	if (choix_monstre == 2)
        	{
        	    printf
        	    ("Heros attaque Monstre, mais Monstre se protege ! Monstre perd 5 PV ! \n");
        	    pv_monstre = pv_monstre - 5;
        	    printf ("Heros : %d PV \n", pv_heros);
        	    printf ("Monstre : %d PV \n", pv_monstre);
        	}
        	if (choix_monstre == 3)
        	{
        	    printf ("Heros attaque Monstre, Monstre perd 20 PV ! \n");
        	    pv_monstre = pv_monstre - 20;
        	    printf ("Monstre empoisonne Heros ! \n");
        	    pm_monstre = pm_monstre - 3;
        	    poison_heros = 1;
        	}
            if (choix_monstre == 4 && feu_monstre == 1)
            {
                printf ("Heros attaque Monstre, Monstre perd 20 PV ! \n");
                pv_monstre = pv_monstre - 20;
                printf ("Le Monstre se soigne du poison ! \n");
                pm_monstre = pm_monstre - 5 ;
		feu_monstre = 0;
            }
    	}
          if (choix == 2)
    	{
    	  if (choix_monstre == 1)
    	  {
    	    printf ("Heros se protege ! \n");
    	    printf ("Monstre attaque ! Mais Heros se protege ! Heros perd 4 PV \n");
    	    pv_heros = pv_heros - 4;
    	    printf ("Heros : %d PV \n", pv_heros);
    	    printf ("Monstre : %d PV \n", pv_monstre);
    	  }
    	  
    	  if (choix_monstre == 2)
    	  {
    	    printf ("Heros se protege ! \n");
    	    printf ("Monstre se protege aussi ! \n");
    	    printf ("Rien ne se passe... \n");
    	    printf ("Heros : %d PV \n", pv_heros);
    	    printf ("Monstre : %d PV \n", pv_monstre);
    	  }
    	  
    	  if (choix_monstre == 3)
    	  {
    	    printf ("Heros attaque Monstre, Monstre perd 20 PV ! \n");
    	    pv_monstre = pv_monstre - 20;
    	    printf ("Monstre empoisonne Heros ! \n");
    	    pm_monstre = pm_monstre - 3;
    	    poison_heros = 1;
    	  }
    	  
    	  if (choix_monstre == 4 && feu_monstre == 1)
    	  {
    	    printf ("Heros se protege ! \n");
    	    printf ("Le Monstre se soigne de son poison ! \n");
    	    pm_monstre = pm_monstre - 5;
	    feu_monstre = 0;
    	  }
    	}
    	
        if (choix == 3)
    	{
    	   if (choix_monstre == 1)
    	   {
    	       printf ("Le Héros embrase le Monstre ! \n");
    	       pm_heros = pm_heros - 3 ;
    	       if (feu_monstre == 1)
    	       {
    	           printf ("Monstre est deja embrasé ! \n");
    	       }
    	       feu_monstre = 1;
    	       printf ("Monstre attaque le Heros, le Heros perd 20 PV ! \n");
    	       pv_heros = pv_heros - 20;
    	   }
    	   
    	   if (choix_monstre == 2)
    	   {
        	   printf ("Le Héros embrase le Monstre ! \n");
        	   pm_heros = pm_heros - 3;
        	   if (feu_monstre == 1)
                {
            	    printf ("Monstre est deja embrasé ! \n");
                }
        	    feu_monstre = 1;
        	    printf ("Le Monstre se protege, mais rien ne se passe... \n");
    	   }
    	       
    	   if (choix_monstre == 3)
        	{
        	    printf ("Le Héros embrase le Monstre ! \n");
        	    if (feu_monstre == 1)
    	        {
    	            printf ("Monstre est deja embrasé ! \n");
    	        }
    	        feu_monstre = 1;
        	    printf ("Monstre empoisonne Heros ! \n");
        	    pm_monstre = pm_monstre - 3;
        	    poison_heros = 1;
        	 }
    	    
    	    if (choix_monstre == 4 && feu_monstre == 1)
    	    {
    	        printf ("Le Héros embrase le Monstre ! \n");
        	    pm_heros = pm_heros - 3;
        	    if (feu_monstre == 1)
                {
            	    printf ("Monstre est deja embrasé ! \n");
                }
                printf ("Le Monstre se soigne de l'embrasement ! \n");
                pm_monstre = pm_monstre - 5;
		feu_monstre = 0;
    	    }
    	}
    	if (choix == 4 && poison_heros == 1)
    	{
    	    if (choix_monstre == 1)
    	    {
    	        printf ("Heros se soigne du poison ! \n");
    	        pm_heros = pm_heros - 5;
		poison_heros = 0;
    	        printf ("Le Monstre attaque le Heros ! Heros perd 20 PV ! \n");
    	        pv_heros = pv_heros - 20;
    	    }
    	
    	    if (choix_monstre == 2)
    	    {
    	        printf ("Heros se soigne du poison ! \n");
    	        pm_heros = pm_heros - 5;
		poison_heros = 0;
    	        printf ("Le Monstre se protege ! Mais rien ne se passe... \n");
    	    }
    	    
    	    if (choix_monstre == 3)
    	    {
    	        printf ("Heros se soigne du poison ! \n");
    	        pm_heros = pm_heros - 5;
		poison_heros = 0;
    	        printf ("Le Monstre empoisonne le Heros ! \n");
    	        pm_monstre = pm_monstre - 3;
		poison_heros = 1;
    	    }
    	    
    	    if (choix_monstre == 4 && feu_monstre == 1)
    	    {
    	        printf ("Heros se soigne du poison ! \n");
    	        pm_heros = pm_heros - 5;
		poison_heros = 0;
    	        printf ("Le Monstre se soigne du poison ! \n");
    	        pm_monstre = pm_monstre - 5;
		feu_monstre = 0;
    	    }
    	}
            printf ("Heros gagne 1 PM \n");
            printf ("Monstre gagne 1 PM \n");
            pm_heros = pm_heros + 1;
            pm_monstre = pm_monstre + 1;
            printf ("Heros : %d PM \n", pm_heros);
            printf ("Monstre : %d PM \n", pm_monstre);
    
        if (feu_monstre == 1)
    	{
    	    printf ("Le Monstre souffre d'un embrasement ! Monstre perd 5 PV ! \n");
    	    pv_monstre = pv_monstre - 5;
    	    printf ("Heros : %d PV \n", pv_heros);
    	    printf ("Monstre : %d PV \n", pv_monstre);
        }
        
        if (poison_heros == 1)
    	{
    	    printf ("Heros souffre du poison ! Heros perd 5 PV ! \n");
    	    pv_heros = pv_heros - 5;
    	    printf ("Heros : %d PV \n", pv_heros);
    	    printf ("Monstre : %d PV \n", pv_monstre);
    	    }
    	    
    	    
    	  /* Début perso 2 *******
    	  *******************
    	  *************
    	  ***********************
    	  *****************
    	  ***************/
    	  
    	  	printf ("Agorran le Guerrier se prépare au combat !");
        printf (" Que faire ? \n (1) Attaquer \n (2) Se defendre \n");
        if (pm_heros >= 3)
    	{
    	   printf ("(3) Trancher l'adversaire \n");
    	}
    	if (pm_heros >= 5)
    	{
    	    printf ("(4) Utiliser un antidote \n");
    	}
        scanf ("%d", &choix);
        choix_monstre = rand () % 2 + 1;
        if (pm_monstre >=5 && feu_monstre == 1)
        {
             choix_monstre = rand () % 4 + 1;
        }
        if (pm_monstre >= 3)
        {
    	    choix_monstre = rand () % 3 + 1;
    	    if (poison_heros == 1)
            {
    	        choix_monstre = rand () % 2 + 1;
            }
    	}
    
        if (choix == 1)
    	{
    	    if (choix_monstre == 1)
    	    {
    	        printf ("Heros attaque Monstre, Monstre perd 20 PV ! \n");
    	        pv_monstre = pv_monstre - 20;
    	        printf ("Monstre contre-attaque ! Heros perd 16 PV ! \n");
    	        pv_heros = pv_heros - 16;
    	        printf ("Heros : %d PV \n", pv_heros);
    	        printf ("Monstre : %d PV \n", pv_monstre);
             }
             
        	if (choix_monstre == 2)
        	{
        	    printf
        	    ("Heros attaque Monstre, mais Monstre se protege ! Monstre perd 5 PV ! \n");
        	    pv_monstre = pv_monstre - 5;
        	    printf ("Heros : %d PV \n", pv_heros);
        	    printf ("Monstre : %d PV \n", pv_monstre);
        	}
        	if (choix_monstre == 3)
        	{
        	    printf ("Heros attaque Monstre, Monstre perd 20 PV ! \n");
        	    pv_monstre = pv_monstre - 20;
        	    printf ("Monstre empoisonne Heros ! \n");
        	    pm_monstre = pm_monstre - 3;
        	    poison_heros = 1;
        	}
            if (choix_monstre == 4 && feu_monstre == 1)
            {
                printf ("Heros attaque Monstre, Monstre perd 20 PV ! \n");
                pv_monstre = pv_monstre - 20;
                printf ("Le Monstre se soigne du poison ! \n");
                pm_monstre = pm_monstre - 5 ;
		feu_monstre = 0;
            }
    	}
          if (choix == 2)
    	{
    	  if (choix_monstre == 1)
    	  {
    	    printf ("Heros se protege ! \n");
    	    printf ("Monstre attaque ! Mais Heros se protege ! Heros perd 4 PV \n");
    	    pv_heros = pv_heros - 4;
    	    printf ("Heros : %d PV \n", pv_heros);
    	    printf ("Monstre : %d PV \n", pv_monstre);
    	  }
    	  
    	  if (choix_monstre == 2)
    	  {
    	    printf ("Heros se protege ! \n");
    	    printf ("Monstre se protege aussi ! \n");
    	    printf ("Rien ne se passe... \n");
    	    printf ("Heros : %d PV \n", pv_heros);
    	    printf ("Monstre : %d PV \n", pv_monstre);
    	  }
    	  
    	  if (choix_monstre == 3)
    	  {
    	    printf ("Heros attaque Monstre, Monstre perd 20 PV ! \n");
    	    pv_monstre = pv_monstre - 20;
    	    printf ("Monstre empoisonne Heros ! \n");
    	    pm_monstre = pm_monstre - 3;
    	    poison_heros = 1;
    	  }
    	  
    	  if (choix_monstre == 4 && feu_monstre == 1)
    	  {
    	    printf ("Heros se protege ! \n");
    	    printf ("Le Monstre se soigne de son Embrasement ! \n");
    	    pm_monstre = pm_monstre - 5;
	    feu_monstre = 0;
    	  }
    	}
    	
    	
    	if (choix == 3)
    	{
    	    if (choix_monstre == 1)
    	    {
    	        printf ("Le Héros abat sa hache sur le monstre ! Monstre perd 30 PV ! \n");
    	        pv_monstre = pv_monstre - 30;
    	        pm_heros = pm_heros - 3;
    	        printf ("Monstre contre-attaque ! Heros perd 16 PV ! \n");
    	        pv_heros = pv_heros - 16;
    	        printf ("Heros : %d PV \n", pv_heros);
    	        printf ("Monstre : %d PV \n", pv_monstre);
             }
             
        	if (choix_monstre == 2)
        	{
        	    printf
        	    ("Le Héros abat sa hache sur le monstre.. mais Monstre se protege ! Monstre perd 15 PV ! \n");
        	    pv_monstre = pv_monstre - 15;
        	    pm_heros = pm_heros - 3;
        	    printf ("Heros : %d PV \n", pv_heros);
        	    printf ("Monstre : %d PV \n", pv_monstre);
        	}
        	if (choix_monstre == 3)
        	{
        	    printf ("Le Héros abat sa hache sur le monstre ! Monstre perd 30 PV ! \n");
        	    pv_monstre = pv_monstre - 30;
        	    pm_heros = pm_heros - 3;
        	    printf ("Monstre empoisonne Heros ! \n");
        	    pm_monstre = pm_monstre - 3;
        	    poison_heros = 1;
        	}
            if (choix_monstre == 4 && feu_monstre == 1)
            {
                printf ("Le Héros abat sa hache sur le monstre ! Monstre perd 30 PV ! \n");
                pv_monstre = pv_monstre - 20;
                pm_heros = pm_heros - 3;
                printf ("Le Monstre se soigne de l'embrasement ! \n");
                pm_monstre = pm_monstre - 5 ;
		feu_monstre = 0;
            }
     
    	}
    	if (choix == 4 && poison_heros == 1)
    	{
    	    if (choix_monstre == 1)
    	    {
    	        printf ("Heros se soigne du poison ! \n");
    	        pm_heros = pm_heros - 5;
		poison_heros = 0;
    	        printf ("Le Monstre attaque le Heros ! Heros perd 20 PV ! \n");
    	        pv_heros = pv_heros - 20;
    	    }
    	
    	    if (choix_monstre == 2)
    	    {
    	        printf ("Heros se soigne du poison ! \n");
    	        pm_heros = pm_heros - 5;
		poison_heros = 0;
    	        printf ("Le Monstre se protege ! Mais rien ne se passe... \n");
    	    }
    	    
    	    if (choix_monstre == 3)
    	    {
    	        printf ("Heros se soigne du poison ! \n");
    	        pm_heros = pm_heros - 5;
		poison_heros = 0;
    	        printf ("Le Monstre empoisonne le Heros ! \n");
    	        pm_monstre = pm_monstre - 3;
		poison_heros = 1;
    	    }
    	    
    	    if (choix_monstre == 4 && feu_monstre == 1)
    	    {
    	        printf ("Heros se soigne du poison ! \n");
    	        pm_heros = pm_heros - 5;
		poison_heros = 0;
    	        printf ("Le Monstre se soigne du poison ! \n");
    	        pm_monstre = pm_monstre - 5;
		feu_monstre = 0;
    	    }
    	}
    	    /* Début perso 3 *******
    	  *******************
    	  *************
    	  ***********************
    	  *****************
    	  ***************/
    	  	printf ("Solegal l'archère se prépare au combat !");
        printf (" Que faire ? \n (1) Attaquer \n (2) Se defendre \n");
        if (pm_heros >= 3)
    	{
    	   printf ("(3) Flèche persante \n");
    	}
    	if (pm_heros >= 5)
    	{
    	    printf ("(4) Utiliser un antidote \n");
    	}
        scanf ("%d", &choix);
        choix_monstre = rand () % 2 + 1;
        if (pm_monstre >=5 && feu_monstre == 1)
        {
             choix_monstre = rand () % 4 + 1;
        }
        if (pm_monstre >= 3)
        {
    	    choix_monstre = rand () % 3 + 1;
    	    if (poison_heros == 1)
            {
    	        choix_monstre = rand () % 2 + 1;
            }
    	}
    
        if (choix == 1)
    	{
    	    if (choix_monstre == 1)
    	    {
    	        printf ("Heros attaque Monstre, Monstre perd 20 PV ! \n");
    	        pv_monstre = pv_monstre - 20;
    	        printf ("Monstre contre-attaque ! Heros perd 16 PV ! \n");
    	        pv_heros = pv_heros - 16;
    	        printf ("Heros : %d PV \n", pv_heros);
    	        printf ("Monstre : %d PV \n", pv_monstre);
             }
             
        	if (choix_monstre == 2)
        	{
        	    printf
        	    ("Heros attaque Monstre, mais Monstre se protege ! Monstre perd 5 PV ! \n");
        	    pv_monstre = pv_monstre - 5;
        	    printf ("Heros : %d PV \n", pv_heros);
        	    printf ("Monstre : %d PV \n", pv_monstre);
        	}
        	if (choix_monstre == 3)
        	{
        	    printf ("Heros attaque Monstre, Monstre perd 20 PV ! \n");
        	    pv_monstre = pv_monstre - 20;
        	    printf ("Monstre empoisonne Heros ! \n");
        	    pm_monstre = pm_monstre - 3;
        	    poison_heros = 1;
        	}
            if (choix_monstre == 4 && feu_monstre == 1)
            {
                printf ("Heros attaque Monstre, Monstre perd 20 PV ! \n");
                pv_monstre = pv_monstre - 20;
                printf ("Le Monstre se soigne du poison ! \n");
                pm_monstre = pm_monstre - 5 ;
		feu_monstre = 0;
            }
    	}
          if (choix == 2)
    	{
    	  if (choix_monstre == 1)
    	  {
    	    printf ("Heros se protege ! \n");
    	    printf ("Monstre attaque ! Mais Heros se protege ! Heros perd 4 PV \n");
    	    pv_heros = pv_heros - 4;
    	    printf ("Heros : %d PV \n", pv_heros);
    	    printf ("Monstre : %d PV \n", pv_monstre);
    	  }
    	  
    	  if (choix_monstre == 2)
    	  {
    	    printf ("Heros se protege ! \n");
    	    printf ("Monstre se protege aussi ! \n");
    	    printf ("Rien ne se passe... \n");
    	    printf ("Heros : %d PV \n", pv_heros);
    	    printf ("Monstre : %d PV \n", pv_monstre);
    	  }
    	  
    	  if (choix_monstre == 3)
    	  {
    	    printf ("Heros attaque Monstre, Monstre perd 20 PV ! \n");
    	    pv_monstre = pv_monstre - 20;
    	    printf ("Monstre empoisonne Heros ! \n");
    	    pm_monstre = pm_monstre - 3;
    	    poison_heros = 1;
    	  }
    	  
    	  if (choix_monstre == 4 && feu_monstre == 1)
    	  {
    	    printf ("Heros se protege ! \n");
    	    printf ("Le Monstre se soigne de son Embrasement ! \n");
    	    pm_monstre = pm_monstre - 5;
	    feu_monstre = 0;
    	  }
    	}
    	
    	
    	if (choix == 3)
    	{
    	    if (choix_monstre == 1)
    	    {
    	        printf ("Le Héros décoche une flèche à pleine vitesse ignorant la défense ! Monstre perd 20 PV ! \n");
    	        pv_monstre = pv_monstre - 20;
    	        pm_heros = pm_heros - 3;
    	        printf ("Monstre contre-attaque ! Heros perd 16 PV ! \n");
    	        pv_heros = pv_heros - 16;
    	        printf ("Heros : %d PV \n", pv_heros);
    	        printf ("Monstre : %d PV \n", pv_monstre);
             }
             
        	if (choix_monstre == 2)
        	{
        	    printf
        	    ("Le Héros décoche une flèche à pleine vitesse ignorant la défense ! Monstre perd 20 PV ! \n");
        	    pv_monstre = pv_monstre - 20;
        	    pm_heros = pm_heros - 3;
        	    printf ("Heros : %d PV \n", pv_heros);
        	    printf ("Monstre : %d PV \n", pv_monstre);
        	}
        	if (choix_monstre == 3)
        	{
        	    printf ("Le Héros décoche une flèche à pleine vitesse ignorant la défense ! Monstre perd 20 PV ! \n");
        	    pv_monstre = pv_monstre - 20;
        	    pm_heros = pm_heros - 3;
        	    printf ("Monstre empoisonne Heros ! \n");
        	    pm_monstre = pm_monstre - 3;
        	    poison_heros = 1;
        	}
            if (choix_monstre == 4 && feu_monstre == 1)
            {
                printf ("Le Héros décoche une flèche à pleine vitesse ignorant la défense ! Monstre perd 20 PV ! \n");
                pv_monstre = pv_monstre - 20;
                pm_heros = pm_heros - 3;
                printf ("Le Monstre se soigne de l'embrasement ! \n");
                pm_monstre = pm_monstre - 5 ;
		feu_monstre = 0;
            }
     
    	}
    	if (choix == 4 && poison_heros == 1)
    	{
    	    if (choix_monstre == 1)
    	    {
    	        printf ("Heros se soigne du poison ! \n");
    	        pm_heros = pm_heros - 5;
		poison_heros = 0;
    	        printf ("Le Monstre attaque le Heros ! Heros perd 20 PV ! \n");
    	        pv_heros = pv_heros - 20;
    	    }
    	
    	    if (choix_monstre == 2)
    	    {
    	        printf ("Heros se soigne du poison ! \n");
    	        pm_heros = pm_heros - 5;
		poison_heros = 0;
    	        printf ("Le Monstre se protege ! Mais rien ne se passe... \n");
    	    }
    	    
    	    if (choix_monstre == 3)
    	    {
    	        printf ("Heros se soigne du poison ! \n");
    	        pm_heros = pm_heros - 5;
		poison_heros = 0;
    	        printf ("Le Monstre empoisonne le Heros ! \n");
    	        pm_monstre = pm_monstre - 3;
		poison_heros = 1;
    	    }
    	    
    	    if (choix_monstre == 4 && feu_monstre == 1)
    	    {
    	        printf ("Heros se soigne du poison ! \n");
    	        pm_heros = pm_heros - 5;
		poison_heros = 0;
    	        printf ("Le Monstre se soigne du poison ! \n");
    	        pm_monstre = pm_monstre - 5;
		feu_monstre = 0;
    	    }
    	  
    	}
            printf ("Heros gagne 1 PM \n");
            printf ("Monstre gagne 1 PM \n");
            pm_heros = pm_heros + 1;
            pm_monstre = pm_monstre + 1;
            printf ("Heros : %d PM \n", pm_heros);
            printf ("Monstre : %d PM \n", pm_monstre);
    
        if (feu_monstre == 1)
    	{
    	    printf ("Le Monstre souffre d'un embrasement ! Monstre perd 5 PV ! \n");
    	    pv_monstre = pv_monstre - 5;
    	    printf ("Heros : %d PV \n", pv_heros);
    	    printf ("Monstre : %d PV \n", pv_monstre);
        }
        
        if (poison_heros == 1)
    	{
    	    printf ("Heros souffre du poison ! Heros perd 5 PV ! \n");
    	    pv_heros = pv_heros - 5;
    	    printf ("Heros : %d PV \n", pv_heros);
    	    printf ("Monstre : %d PV \n", pv_monstre);
    	  
        }
    }

    if (pv_monstre <= 0)
    {
        printf (" Monstre n'a plus de PV, Heros gagne !");
    }
    
    if (pv_heros <= 0)
    {
        printf ("Heros n'a plus de PV, Monstre gagne...");
    }
    return 0;
}

