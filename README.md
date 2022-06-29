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
**id** | L'ID unique du spot.
user_id | ID de l'utilisateur qui a ajouté le spot.
name | Nom du spot
description | Description du spot
longitutde | Coordonnées du spot 
latitude | Coordonnées du spot 
like | Nombre de like

```javascript
{
  "id" : "1",
  "user_id" : "fazKUHrerXeTSB74lW2evVZmLBr1",
  "name" : "Pont Alexandre III au coucher du soleil",
  "description" : "Découvrez le pont sous un tout nouvel angle",
  "longitutde" : "49.4993838",
  "latitude" : "41.4320044",
  "like" : "321"
}
```


