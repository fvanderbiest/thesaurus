10/08/2015
Ma�l REBOUX - Rennes M�tropole pour le p�le m�tier INSPIRE de G�oBretagne

URBAMET est un thesaurus est tr�s connu des urbanistes mais nous n�avons jamais pu g�rer ses mots-cl�s dans nos catalogue car il n�existe pas de version RDF/ SKOS disponible.

J�ai r�ussi � r�cup�rer aupr�s du Minist�re de l��cologie un export en XML du thesaurus URBAMET.
http://notx.documentation.developpement-durable.gouv.fr/Urbanisme/thesaurus/navigation.xhtml 

Le jeu est de traiter ce fichier pour cr�er un fichier XML RDF / SKOS.


J�ai � peu pr�s r�ussi mais il reste � traiter la hi�rarchie entre les termes pour que ce soit op�rationnel.
Pour ceux � qui �a parle, il s�agit des descripteur narrower et broader. C�est obligatoire pour avoir un fichier SKOS valide.
Je me sers de thmanager pour valider. J�ai proc�d� ainsi pour le thesaurus de G�oBretagne (non hi�rarchique) et mes 2 th�saurus internes (dont 1 hi�rarchique).

Et l� je ne sais pas trop comment m�y prendre en terme de m�thodologie donc j�appelle � l�aide !

Je pense qu�il faut faire en 3 �tapes. La premi�re est faite cf le script python et les r�sultats.
La 2e consisterait � reparcourir tous les concepts / mot-cl�s et � �tablir les relations parents-enfants.
La 3e consisterait � refaire un parcours pour d�terminer les relations de voisinage (termes au m�me niveau / sous le m�me terme).

