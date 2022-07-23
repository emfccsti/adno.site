---
title: "Mode d'emploi"
date: 2022-05-25T13:18:58+02:00
type: page
---

## Pour commencer

Adno est un projet d'éditeur / visualiseur d'images IIIF. A terme, il permettra d'annoter et de créer des parcours sur ces images, de les partager aussi.


Pour l'heure, en page d'accueil, il est seulement possible de créer des annotations, de les visualiser, de les modifier, mais pas de les enregistrer.

Créer des annotations
: Touche `Maj` puis cliquer-glisser pour sélectionner une zone, éventuellement saisir une note, puis enregistrer en cliquant sur `OK`.

## Qu'est-ce que IIIF ?

Le but de IIIF (International Image Interoperability Framework) est de fournir un cadre technique commun grâce auquel les bibliothèques numériques peuvent diffuser leurs images de manière standardisée sur le Web afin de les rendre consultables, manipulables et annotables par n’importe quelle application ou logiciel compatible. IIIF favorise l'interopérabilité et offre une expérience utilisateur enrichie en termes d'accès, de manipulation et d'exploitation des images.

Pour en savoir plus, consultez le site officiel [iiif.io](https://iiif.io), en anglais, ou, en français, le portail [Biblissima](https://iiif.biblissima.fr/), qui constitue un excellent point d'entrée pour comprendre et expérimenter IIIF.

## Exemples

Par défaut :
- __Siège de Poitiers par Coligny en 1569__, peinture de François Nautré,
Musées de la ville de Poitiers et de la Société des Antiquaires de l'Ouest  
[https://free.iiifhosting.com/iiif/1c8d49343676a04fffcd92979c02e9394e48bac96f590fffbadffc9133cd06b9/info.json](https://adno.app?url=https://free.iiifhosting.com/iiif/1c8d49343676a04fffcd92979c02e9394e48bac96f590fffbadffc9133cd06b9/info.json)

Vous pouvez entrer votre propre image IIIF

{{< rawhtml >}}
<form action="/" method="get">
  <input type="url" id="url" name="url" placeholder="URL info.json d'une image IIIF" style="width: 80%">
  <input type="submit" value="Voir">
</form>
{{< /rawhtml >}}

Ou encore essayer une des images suivantes :
- __Atelier d'idéation d'Adno__ par les participants à la réunion du 23 juin  
[https://iiif.emf.fr/iiif/3/ideation.jpg/info.json](https://adno.app/?url=https://iiif.emf.fr/iiif/3/ideation.jpg/info.json) 
- __Voûte de l'abbaye de Saint-Savin__  
[https://iiif.emf.fr/iiif/3/saint-savin.jpg/info.json](/?url=https://iiif.emf.fr/iiif/3/saint-savin.jpg/info.json)
- __Tite-Live, Histoire romaine, version française par Pierre Bersuire__ Manuscrits de la Bibliothèque Sainte-Geneviève.    
[https://gallica.bnf.fr/iiif/ark:/12148/btv1b6001280q/f19/info.json](/?url=https://gallica.bnf.fr/iiif/ark:/12148/btv1b6001280q/f19/info.json)
- __Table de Peutinger (Tabula Peutingeriana)__ Copie du XIIIe siècle d'une ancienne carte romaine où figurent les routes et les villes principales de l'Empire romain, fac-similé de Konrad Miller de 1887.  
[https://iiif.emf.fr/iiif/3/peutinger.jp2/info.json](/?url=https://iiif.emf.fr/iiif/3/peutinger.jp2/info.json)
- __Panorama de Hong Kong__ par [Mark Lehmkuhler](https://www.flickr.com/photos/mark_lehmkuhler/33011219102), prise de vue par drone.  
[https://iiif.emf.fr/iiif/3/HongKong.jp2/info.json](/?url=https://iiif.emf.fr/iiif/3/HongKong.jp2/info.json)
- __Tapisserie de Bayeux__ Voir aussi [ici la version restaurée](https://www.bayeuxmuseum.com/la-tapisserie-de-bayeux/decouvrir-la-tapisserie-de-bayeux/explorer-la-tapisserie-de-bayeux-en-ligne/)  
[https://iiif.lib.ncsu.edu/iiif/xx-bayeux/info.json](/?url=https://iiif.lib.ncsu.edu/iiif/xx-bayeux/info.json)
- __Mountains & Rivers in th World__ Première édition par G.W. Colton en 1849 de cette représention iconique des principales montagnes et rivières du monde.  
[https://iiif.emf.fr/iiif/3/coltons-mountains-rivers-infographic-map.jp2/info.json](?url=https://iiif.emf.fr/iiif/3/coltons-mountains-rivers-infographic-map.jp2/info.json)
[https://iiif.emf.fr/iiif/3/SARS-CoV-2.jp2/info.json](/?url=https://iiif.emf.fr/iiif/3/SARS-CoV-2.jp2/info.json)
- __Chat "regardant" à travers une longue-vue et autre chat perché dessus (Agence Rol)__ BnF, département Estampes et photographie, EST EI-13 (89).  
[https://gallica.bnf.fr/iiif/ark:/12148/btv1b69162903/f1/info.json](/?url=https://gallica.bnf.fr/iiif/ark:/12148/btv1b69162903/f1/info.json)
- __Un souvenir de vacances__ Une « planche de science » réalisée par Camille Arnoult du lycée Camille Jullian (Bordeaux).  
[https://iiif.emf.fr/iiif/3/UnSouvenirDeVacances.jp2/info.json](/?url=https://iiif.emf.fr/iiif/3/UnSouvenirDeVacances.jp2/info.json)

Les images précédentes sont fournies par des serveurs IIIF. Cepandant, il est possible de s'en passer et de fournir une image statique IIIF composée d'un fichier `info.json` et d'une arborescence de tuiles. Cf. ce [tuto](http://ronallo.com/iiif-workshop-new/image-api/image-servers/static.html).
- __Étoiles de mer__ Image statique IIIF. Voir la structure à [cette adresse](https://static.emf.fr/adno/static/iiif/starfish/)   
[https://static.emf.fr/adno/static/iiif/starfish/info.json](https://adno.app/?url=https://static.emf.fr/adno/static/iiif/starfish/info.json)

Il est possible d'utiliser des images autres que IIIF
- __Sonde Cassini__ DZI (Deep Zoom Image). Voir la structure à [cette adresse](https://static.emf.fr/adno/static/dzi/)  
[https://static.emf.fr/dev/dzi/cassini.dzi](https://adno.app/?url=https://static.emf.fr/adno/static/dzi/cassini.dzi)
- __Mario__ image statique au format png  
[https://www.pngmart.com/files/2/Mario-PNG-Image.png](https://adno.app/?url=https://www.pngmart.com/files/2/Mario-PNG-Image.png)
- __Panorama de Poitiers__ image statique au format jpg (Lucas Aless)  
[https://upload.wikimedia.org/wikipedia/commons/1/1d/Poitiers_panorama_01.jpg](https://adno.app?url=https://upload.wikimedia.org/wikipedia/commons/1/1d/Poitiers_panorama_01.jpg)

## Adno repose sur des logiciels libres

Adno utilise les composants libres existants, notamment [OpenSeaDragon](https://openseadragon.github.io/) comme visualiseur et [Annotorious](https://recogito.github.io/annotorious/) pour créer les annotations.
