# Mapview

Présentation du projet: le but du projet était d'automatiser le défilement de cartes qliksense qui affiche 
le déplacement des bateaux de l'entreprise. Il faut egalement automatiser le rechargement des données qui 
sont recupérés grace a un logiciel spécifique. Ce projet a pour but de simplifier la tache des salariés afin qu'ils n'aient plus 
besoin de chercher par eux même leurs bateaux le projet montre aussi des cartes des vents et vagues.


Les outils mis en oeuvre:
* Qliksense
* Autoit
* Reuters
* Excel

Le developpement tourne autour de 2 grandes parties

1. L'autoit de Reuters et du ficher excel
2. L'autoit de Qliksense


|Développement                             |Langages|Technique de programmation             |
|------------------------------------------|--------|---------------------------------------|
|Automatisation du rechargement des données|Autoit  |Developpement d'une application Autoit |
|Automatisation du défilement des cartes   |Autoit  |Developpement d'une application Autoit |                                      |




Procédure AutoIt et manuel d’instruction Qliksense

Sommaire :
1)	Procédure autoit Reuters
2)	Procédure autoit Qliksense 
3)	User et mot de passe Qliksense 
4)	Défilement des cartes sur Qliksense et google 
5)	En cas de problème 
6)	Etape pour déployer Mapview sur un autre pc 


# 1)Procédure autoit Reuters :

ATTENTION : NE PAS TOUCHER AU CLAVIER OU A LA SOURIS LORS DU DEROULEMENT DU PROGRAMME TOUT EST FAIT AUTOMATIQUEMENT.

Le programme Autoit sert à la mise en route de Reuters puis une ouverture du fichier Excel afin d’obtenir les données le plus récentes sur les bateaux (Localisation).
1)	Ouverture de REUTERS. (Si l’utilisateur n’est pas le Sign in il le fait automatiquement)
2)	Laisse le temps à Reuters de se lancer. (20 sec)
3)	Ouvre le fichier Excel avec les différents DWT
4)	Refresh le fichier Excel afin d’avoir les données les plus récentes
5)	Ferme le fichier Excel 
6)	Ferme Reuters

Google drive :
Tous les fichiers sont mis dans Google drive de sorte que l’accès soit plus simple.
Chemin pour accéder au fichier Excel :
Google Drive>Dreyfus_qlikview_app>MAPVIEW>xls>Mapview_Reuters


# 2)Procédure autoit Qliksense:
ATTENTION : NE PAS TOUCHER AU CLAVIER OU A LA SOURIS LORS DU DEROULEMENT DU PROGRAMME TOUT EST FAIT AUTOMATIQUEMENT.

ATTENTION NE LANCEZ PAS IMMEDIATEMENT L’AUTOIT AU LORSQUE VOUS ALLUMEZ L’ORDINATEUR ATTENDEZ QU’IL SOIT BIEN CONNECTEZ AU RESEAU.

Le programme sert à afficher le déplacement des bateaux en temps réel sur différentes cartes qui défile automatiquement.
 Allumer l’ordinateur une fois sur le bureau cliquer sur l’icône du nom de Mapview.exe puis laisser tourner le programme.
 
 
Laissez le temps au programme de s’exécuter une action ne prend pas plus d’une minute si vous trouvez que l’écran reste figé trop longtemps attendez. 
Le temps est long en raison de la connexion qui peut parfois être plus lente que prévu.

Déroulement du programme :
1)	Lancement de l’application Google Wind (10-35 sec)
2)	Lancement de QlikSense (10-30 sec)
3)	Lancement de l’application Mapview (10-15 sec)
4)	Lancement du récit (10-15 sec)
5)	Durée du diaporama (1800 sec pour 200 sec par slide)
6)	TOUTES LES 6 HEURES : Chargement des données (40-60 sec)
7)	Durée de l’affichage des cartes winds et waves (100 sec)
8)	Temps que le boucle d’affichage des cartes met : environ 1920 sec 

	
# 3) User et mot de passe Qliksense: 
             user : Mapview2019
				     MDP : ***********


# 4)Défilement des cartes sur Qliksense et google 

Si une carte QlikSense passe alors que vous êtes en train de la regarder il suffit d’appuyer sur CONTROL puis la touche flèche de gauche du clavier a l’inverse si vous voulez passer à la slide suivante appuyez CONTROL puis sur flèche de droite.
Pour les cartes google il suffit de faire {CTRL}+{TAB}

ATTENTION APPPUYEZ SUR LES FLECHES UNIQUEMENT SI LES CARTES S’AFFICHE SINON NE TOUCHEZ A RIEN.

# 5) En cas de problème

En cas de problème avec l’exécution de l’Autoit fermer le programme en appuyant sur la touche ECHAP, éteignez l’ordinateur (ainsi que toutes les applications ouvertes. 
Sauvegardez si nécessaire) et rallumez-le normalement puis relancer le programme.

Si vous êtes sur une tablette Windows ou il y’a la touche FN faites : fn puis echap
Si vous voulez stopper le programme sans fermer les applications appuyer la touche {$}.


# 6) Etape pour déployer Mapview sur un autre pc :
1)	Installer Qliksense et Autoit (gratuit)
2)	Installer google drive sur le pc ( mail :ldacetramax@gmail.com , mdp : *************
3)	Une fois les fichiers installés ouvrer le google drive et qlik sense
4)	Connecté vous a qliksense vous arrivez sur le dossier avec tout les projet 
5)	Faites copier-coller du fichier Mapview_V4.qvf situer dans google drive :
Dreyfus_qlikview_app->MAPVIEW->Sense->Apps 
Puis copier le dans le disque local : C:\Users\*utilisateur*\Documents\Qlik\Sense\Apps
6)	Allez ensuite sur le dossier autoit de google drive :
Dreyfus_qlikview_app->MAPVIEW->Autoit
Faites glisser l’icône  avec écrit mapview.exe sur le bureau.
 
7)	Fermer toutes les applications et cliquer sur l’icone que vous venez de mettre sur le bureau.		
