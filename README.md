# JEE-web-developpement-first-jstl

https://openclassrooms.com/fr/courses/2434016-developpez-des-sites-web-avec-java-ee/2438626-jstl-et-variables

you can change the source code in bonjour.jsp exacly between body tags like this:

On affiche une variable en JSTL de la façon suivante :

<p><c:out value="${ variable }">Valeur par défaut</c:out></p>
On peut directement y définir une variable, avec son champ d'application :

<c:set var="pseudo" value="Mateo21" scope="page" />
On peut supprimer la variable :

<c:remove var="pseudo" scope="page" />
On peut travailler aussi avec des Java Beans. Ici, on modifie la propriété d'un Bean puis on l'affiche :

<c:set target="${ auteur }" property="prenom" value="Mathieu" />
<p><c:out value="${ auteur.prenom }" /></p>
