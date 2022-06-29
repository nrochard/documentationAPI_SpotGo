# documentationAPI_SpotGo

## Overview

Étant un profil de développeuse front, j'ai décidé d'utiliser Firebase pour mon application SpotGo afin de consacrer plus de temps sur le front. L'application n'étant pas complexe, j'ai choisi cette solution plus simple à utiliser. 

### Users

Champs | Description
------|------------
**id** | L'ID unique de l'utilisateur.
name | Le nom de l'utilisateur.
phone | Le numéro de téléphone de l'utilisateur
created_at | Date de création de l'utilisateur
is_subscribed | État de l'abonnement

```javascript
{
  "id" : "fazKUHrerXeTSB74lW2evVZmLBr1",
  "name" : "noemie_rochard",
  "phone" : "+33606808704",
  "created_at" : 2022-06-21,
  "is_subscribed" : 0
}
```

### Spots

Champs | Description
------|------------
**id** | L'ID unique du spot
user_id | ID de l'utilisateur qui a ajouté le spot.
name | Nom du spot
description | Description du spot
tutorial | Tutoriel du spot
longitude | Coordonnées du spot 
latitude | Coordonnées du spot 
like | Nombre de like

```javascript
{
  "id" : "1",
  "user_id" : "fazKUHrerXeTSB74lW2evVZmLBr1",
  "name" : "Pont Alexandre III au coucher du soleil",
  "description" : "Découvrez le pont sous un tout nouvel angle",
  "tutorial" : "J'ai réalisé cette photo avec un GH5. Venez avant 8h, car le lieu est peu fréquenté à ce moment."
  "description" : "Découvrez le pont sous un tout nouvel angle",
  "longitutde" : "49.4993838",
  "latitude" : "41.4320044",
  "like" : "321"
}
```

### Collections

Champs | Description
------|------------
**id** | L'ID unique de la collection
user_id | ID de l'utilisateur à qui appartient la collection
name | Nom de la collection
spot_id | Id des spots 

```javascript
{
  "id" : "1",
  "user_id" : "fazKUHrerXeTSB74lW2evVZmLBr1",
  "name" : "Shooting Paris",
  "spot_id" : "{0: '34', 1: '29'}",
}
```

### Favorites

Champs | Description
------|------------
**id** | L'ID unique des favoris
user_id | ID de l'utilisateur à qui appartient les favoris
spot_id | Id des spots 

```javascript
{
  "id" : "1",
  "user_id" : "fazKUHrerXeTSB74lW2evVZmLBr1",
  "spot_id" : "{0: '1', 1: '90'}",
}
```

### Comments

Champs | Description
------|------------
**id** | L'ID unique du commentaire
user_id | ID de l'utilisateur qui a rédigé le commentaire
spot_id | Id du spot auquel le commentaire est associé  
content | Texte du commentaire

```javascript
{
  "id" : "1",
  "user_id" : "fazKUHrerXeTSB74lW2evVZmLBr1",
  "spot_id" : "43",
  "content" : "Je recommande vivement ce spot, il est très peu fréquenté"
}
```
