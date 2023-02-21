
Le langage HTML est un langage à balises, comme son nom l’indique : HyperText Markup Language, Langage à
Balises Hypertextes. Notez aussi que le HTML est originellement une application SGML (Standard Generalized Markup
Language).
Le langage HTML est saisi dans un document de type texte, ayant pour extension .html. Le HTML est interprété par un « agent utilisateur » pour reprendre la terminologie officielle (user agent). Ces agents utilisateurs du HTML sont la plupart du temps des navigateurs web, mais il existe d’autres formes d’applications capables d’interpréter le HTML,
comme les lecteurs d’écran audio, les robots d’indexation des moteurs de recherche, mais aussi des systèmes embarqués dans des appareils électroniques.
L’objectif du HTML est de décrire la structure des pages web et d’indiquer le contenu sémantique de chaque élément constitutif de ces pages. Le HTML décrit le contenu des pages web à l’aide d’éléments HTML qui sont constitués de balises. Chaque élément est dédié à l’affichage d’un type de contenu donné. Vous avez des éléments HTML qui affichent les titres, les images, les tableaux, les formulaires…
Le HTML est donc bien un langage sémantique : chaque élément doit être utilisé dans le cadre de sa définition et les agents utilisateurs attendent un contenu donné pour chaque élément. Par exemple, l’élément HTML <p> est fait pour contenir un paragraphe de texte et non un tableau, l’élément HTML <img> est fait pour contenir une image et non un champ de formulaire. Pour que vos pages web soient valides et bien interprétées par les navigateurs, vous devez respecter cette sémantique.

HTML signifie HyperText Markup Language


Un element HTML est compose d'une balise d'ouverture et d'une balise de fermeture: 
``` html
    <p> contenu </p>
```
Il faut noter que certains elements HTML n'ont pas de balise fermante : 
``` html
<hr>
```

Chaque element HTML peut avoir un ou plusieurs attributs : 

``` html
    <p id="test" > ceci est un paragraphe </p>

    <img src="images/images.jpg" alt="image not found!" title="Titre de l'image">
```



L'element `<html>` est l'element racine des pages HTML


L'element head : 

Il contient des proprietes essentielles pour les pages web.

Chacune de ces proprietes est renseigne avec des elements enfants



Conception d'une page web

Pour concevoir vos pages, vous devez réfléchir en termes de « conteneur ». Un conteneur, comme son nom l’indique, inclut un contenu de type très varié.

Dans ces conteneurs, vous pourrez placer du texte, des images, des formulaires, des liens, des tableaux… Mais vous
pourrez aussi avoir des conteneurs plus « petits » comme pour mettre en évidence un ou plusieurs mots, ou pour
définir une cellule de tableau.

Les conteneurs servent aussi à structurer vos pages. Vous pourrez ainsi utiliser des conteneurs pour insérer un entête
de page, une colonne latérale (une sidebar en anglais), un pied de page, une barre de navigation…


#### L'element div

L’élément <div> est un des conteneurs les plus anciens du HTML. Il permet de créer une division structurelle dans la
page. Dans ces divisions, nous pouvons placer n’importe quel contenu et même d’autres conteneurs comme d’autres
divisions <div>, des paragraphes, des listes… Ces divisions permettaient d’effectuer des mises en page à l’aide de
conteneurs "neutres", c’est à dire sans contenu sémantique défini.



#### L'element span 

L’élément <span> est souvent utilisé, par exemple, pour avoir une division au sein d’un paragraphe de texte. Ceci est très pratique pour mettre en forme de manière particulière du texte dans un texte formaté d’une autre manière.


#### L'element header

L’élément `<header>` permet d’insérer une zone d’affichage pour les entêtes.
Ces entêtes peuvent être utilisés à plusieurs endroits :
- au niveau de la page, c’est l'entête de page classique, souvent placé en haut de l’écran, avec un logo, un slogan, une barre de navigation principale...


#### L'element footer:
L’élément `<footer>` permet d’insérer une zone d’affichage pour les pieds de page. Nous retrouvons la même
sémantique que pour les entêtes.
Ces pieds de page peuvent être définis pour la page ou pour une autre zone d’affichage de celle ci, comme un article. Notez que l’usage d’un `<footer>` n’implique pas forcément l’usage d’un `<header>`.

#### L'element nav: 
L’élément `<nav>`, comme son nom le laisse supposer, est dédié à l’affichage d’une barre de navigation avec des liens
hypertextes. Mais attention, ne vous sentez pas obligé de n’avoir qu’une seule zone de navigation par page. Vous
pouvez créer autant d’éléments `<nav>` que vous avez de navigations différentes dans vos pages, à partir du
moment où chacun d’entre eux est bien identifié. L’élément `<nav>` est plutôt dédié à la navigation principale du site,
à la création de liens entre les pages du site.
Vous pouvez inclure une navigation principale `<nav>` dans un entête
`<header>` et une navigation secondaire
`<nav>` dans un pied de page `<footer>`, par exemple.

#### L'element main: 

L’élément `<main>` permet d’indiquer le contenu principal de la page. Ce contenu doit être unique et ne pas être
répété dans la page. De plus, le W3C indique précisément son contexte d’utilisation : il ne doit pas être utilisé à
l’intérieur, comme élément inclus, dans les éléments `<article>`, `<aside>`, `<footer>`, `<header>` ou `<nav>`.

#### L'element section: 

L’élément <section> permet de regrouper des éléments partageant une même thématique. Cela permet de
regrouper dans un même élément un contenu structuré, avec son entête
et son pied de page. L’utilisation de
plusieurs éléments <section> distinguera plusieurs parties, plusieurs sections au sein d’une même page, avec
d’autres éléments de structure imbriqués.

#### Les balises titres : cf code

#### Les listes

Liste non ordonnee
```
<ul>
    <li>lorem</li>
    <li>ipsum</li>
    <li>foo bar</li>
</ul>
```

Liste  ordonnee
```
<ol start="4" type="I" >
    <li>lorem</li>
    <li>ipsum</li>
    <li>foo bar</li>
</ol>
```


##### Insertion de liens pour les pages web

Par essence même, le Web est constitué de liens hypertextes : les pages sont reliées par des liens hypertextes. Et le
HTML contient bien le mot hypertexte dans son abréviation, il correspond au H de HyperText Markup Language.
Vous allez pouvoir lier des pages entre elles, d’un site à l’autre, mais aussi au sein d’une même page de votre site.
Vous insérerez des liens vers des adresses de messagerie, vers des réseaux sociaux et pour télécharger des fichiers
par exemple.
Enfin, notez que les liens sont des éléments de type en ligne (inline).


La structure d'un lien html 

On utilise la balise `<a></a>` pour inserer des liens


Les liens que vous allez insérer auront plusieurs destinations possibles. Ils peuvent cibler une page de votre site ou une page d’un autre site. Dans le premier cas, l’URL pourra être relative, dans le second, l’URL devra être absolue.



#### Utilisation des images en HTML

L’élément `<img>` est fait pour insérer des images d’illustration directement liées au contenu rédactionnel. D’un point
de vue sémantique, cet élément n’est pas fait pour appliquer une image de fond à un entête
ou toute autre zone
d’affichage dans la page. Pour cela, il faut utiliser une règle CSS.

L'attribut src permet de specifier le chemin d'acces vers l'image qu'on souhaite afficher.


#### Les formulaires en HTML 

Les formulaires sont insérés dans l’élément `<form>`. Dans cet élément, nous trouverons tous les champs utiles et les boutons de validation et d’annulation.

Les attributs acceptes par l'element form: 
- action: indique l'URL qui va prendre en charge les donnees saisies par le formulaire
- method: specifie si les donnees seront envoyes via http avec la methode GET ou POST.
- name: le nom du formulaire
- enctype: indique le type MIME des donnees envoyees.

https://developer.mozilla.org/fr/docs/Web/HTTP/Basics_of_HTTP/MIME_types/Common_types




### Le role du CSS



On peut appliquer du style a certains elements a l'aide l'attribut class. En CSS on cible les elements dont la classe est test de la maniere suivante: 
``` CSS
.test {
    test-transform: uppercase;
}
```

On peut aussi en CSS appliquer du style de maniere specifique grace a l'attribut html id: 
``` CSS
#test {
    /* ceci est un commentaire  */
}
```


#### Structure et regles du CSS

Ceci est une regle de style: 
```
selecteur {
    props: valeur
}
```

Les selecteurs : 
- ne doivent pas commencer par un chiffre
- ne peuvent pas contenir d'espace, de caracteres speciaux, de caracteres avec accents
-  peuvent contenir des `-` et  des `_`
- sont sensibles a la casse (majuscule/minuscule)


Les expressions regulieres
Lien : https://developer.mozilla.org/fr/docs/Glossary/Regular_expression



#### Les selecteurs de pseudo-classes: 

Les pseudoclasses permettent de cibler des éléments qui ne sont pas accessibles avec les sélecteurs classiques
et qui prennent un état particulier, comme les liens visités. En ce qui concerne la syntaxe, une pseudoclasse commence toujours par le caractère deux points : et est immédiatement suivie par le nom de la pseudoclasse.


Pour cet apres-midi : 

- Preparer la maquette de votre futur site web

- Se documenter sur les outils css Bootstrap / Flexbox et CSSGRid 
- Utiliser un (ou plusieurs) de ces outils afin de creer la structure generale de votre (vos) pages web
- Veillez a bien separer les fichiers HTML, CSS et les assets dans des dossiers separes.