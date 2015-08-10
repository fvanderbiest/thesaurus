10/08/2015
Ma�l REBOUX - Rennes M�tropole pour le p�le m�tier INSPIRE de G�oBretagne

Ce script python permet de g�n�rer le thesaurus G�oBretagne v 2.x � partir de la liste des termes (liste_termes.txt).

La liste des termes et leur d�finition est accessible ici : http://kartenn.region-bretagne.fr/wiki/doku.php?id=pole_catalogage:thesaurus_geobretagne

Pour pouvoir �tre utilisable dans GeoNetwork, un thesaurus doit �tre au format RDF / SKOS.
Le seul logiciel libre connu disposant d'une interface graphique permettant de g�n�rer ou manipuler un tel format est thManager.

Apr�s avoir g�n�rer le fichier RDF il convient donc de le charger dans thManager pour le valider. Tr�s important, surtout si le thesaurus est hi�rarchis� / hi�rarchique. Ce qui n'est pas le cas du thesaurus G�oBretagne.

Ne pas oublier de surcharger le fichier produit avec les infos de version. thManager ne sait pas les lire mais GeoNetwork oui : elles apparaissent devant les mot-cl�s dans l'interface lors de la consultation d'une m�tadonn�e.


++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

<?xml version="1.0" encoding="UTF-8"?>
<!-- 
  Thesaurus G�oBretagne
  version 2.0 du 13/01/2014
-->
<rdf:RDF
    xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"
    xmlns:skos="http://www.w3.org/2004/02/skos/core#"
    xmlns:dc="http://purl.org/dc/elements/1.1/"
    xmlns:foaf="http://xmlns.com/foaf/0.1/"
    xmlns:dcterms="http://purl.org/dc/terms/" >
  <skos:ConceptScheme rdf:about="http://www.geobretagne.fr/thesaurus">
    <dc:title>G�oBretagne v 2.0</dc:title>
    <dc:description>Thesaurus de la nomenclature th�matique de G�oBretagne pour GeoNetwork.</dc:description>
    <dc:creator>
      <foaf:Organization>
        <foaf:name>G�oBretagne</foaf:name>
      </foaf:Organization>
    </dc:creator>
    <dcterms:issued>2014-01-13</dcterms:issued>
    <dcterms:modified>2014-01-13</dcterms:modified>
  </skos:ConceptScheme>

++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++