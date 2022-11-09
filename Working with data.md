
Regarder les vidéos de Daniel Shiffman sur l'utilisation des données :
https://www.youtube.com/playlist?list=PLRqwX-V7Uu6a-SQiI4RtIwuOrLJGnel0r


### Exercices

Après avoir regardé une vidéo, faire l'exercice correspondant ci-dessous. 
Attention à ne pas passer plus de 1/2h par exercice et ne pas aller trop loin dans le styling. 

#### 10.3: What is JSON?

* Choisir un set de donnée sur https://github.com/Tressley/hpjson ou https://github.com/dariusk/corpora
* Charger le JSON en local
* Afficher une liste des données récupérées. 
* Envoyer sur discord le lien vers le sketch P5 

#### 10.4: Loading JSON data from a URL (Asynchronous Callbacks!)

* Installer le [[#CORS|proxy cors]]
* Trouver une visualisation sympa (mais rapide, max 1/2h) pour afficher les astronautes dans leur vaisseaux respectifs.
* Eventuellement utiliser https://p5js.org/reference/#/p5/image pour afficher une image du vaisseau.
* Envoyer sur discord le lien vers le sketch P5

### 10.5: Working with APIs in Javascript - p5.js Tutorial

* Se créer un compte sur https://openweathermap.org/
* Recuperer son API key sur https://home.openweathermap.org/api_keys
* En utilisant la prevision à 5 jours https://openweathermap.org/forecast5 pour votre localisation (p.ex : http://api.openweathermap.org/data/2.5/forecast?q=gembloux&appid=TON_API_KEY_ICI  charger les previsions météos en utilisant LoadJSON
* Afficher les temperatures à 5 jours
* BONUS : utiliser https://developer.mozilla.org/fr/docs/Web/API/Geolocation/getCurrentPosition pour récuperer dynamiquement votre position (voir aussi https://www.youtube.com/watch?v=3ls013DBcww&list=PLRqwX-V7Uu6YxDKpFzf_2D84p0cyk4T7X&index=10)
* Envoyer sur discord le lien vers le sketch P5

### 10.6: API Query with User Input

* Dupliquer votre [[#10.5: Working with APIs in Javascript - p5.js Tutorial|exercice précédent]]
* Permettre à l'utilisateur de selectionner sa propre localisation
* Envoyer sur discord le lien vers le sketch P5

### 10.7: API Query with JavaScript setInterval()

* Afficher la position de l'ISS en temps réel sur l'écran.
* En réutilisant les données obtenues lors de l'[[#10.4: Loading JSON data from a URL (Asynchronous Callbacks!)|Exercice 10.4]] afficher le nombre d'astronautes en plus.
* Envoyer sur discord le lien vers le sketch P5

#### Apres les vidéos 

* Explorer le web à la recherche d'API interessantes
* Me soumettre 5 API que vous pouvez interroger pour récuperer des données. Pour chaque API, me donner un exemple du type de donnée que cette API
* A partir de 2 de ces API, imaginer une visualisation créative et me faire un court pitch des 2 idées.
* Envoyer sur discord le lien vers le sketch P5

### Notes

#### Code des exemples

Le dossier https://github.com/CodingTrain/website-archive/tree/main/Tutorials/P5JS/p5.js/10 contient le code des exemples de Dan Shiffman.

#### CORS

Malheureusement, les techniques évoquées par Dan en 2015 pour contourner les limitations liées au CORS en utilisant JSONP ne fonctionnent plus avec les versions actuelles des navigateurs.

Pour pallier à cette limitation, j'ai implementé un petit serveur nodeJS qui permet d'ajouter des headers CORS aux requetes qui n'en fournissent pas.

Les instructions pour son utilisation se trouvent ici : https://github.com/thylo/iad-cors-proxy

Exemple : https://editor.p5js.org/thylo/sketches/mBCBJ9Hmd
