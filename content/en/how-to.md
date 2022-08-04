---
title: "How to"
date: 2022-08-04T13:18:58+02:00
type: page
translationKey: how-to 
---

## To get started

Adno is a IIIF image editor/viewer project. Eventually, it will allow to annotate and create stories on these images, to share them too.

For the moment, on the home page, it is only possible to create annotations, view them, modify them, but not to save them.

Creating annotations
: `Shift` key then click and drag to select an area, possibly enter a note, then save by clicking on `OK`. 

## What is IIIF ?

The goal of [IIIF](https://iiif.io) (International Image Interoperability Framework) is to provide a common technical framework through which digital libraries can deliver their images in a standardized manner on the Web. So that they can be searched, manipulated, and annotated by any compatible application or software. IIIF promotes interoperability and provides a richer user experience in terms of accessing, manipulating and using images.

To learn more about IIIF, visit the official website [iiif.io](https://iiif.io), in english, or [Biblissima](https://iiif.biblissima.fr/) for a french version, which is an excellent entry point to understand and experiment IIIF.

## Examples 

By défault:
- __Siège de Poitiers par Coligny en 1569__, peinture de François Nautré,
Musées de la ville de Poitiers et de la Société des Antiquaires de l'Ouest  
[https://free.iiifhosting.com/iiif/1c8d49343676a04fffcd92979c02e9394e48bac96f590fffbadffc9133cd06b9/info.json](https://adno.app?url=https://free.iiifhosting.com/iiif/1c8d49343676a04fffcd92979c02e9394e48bac96f590fffbadffc9133cd06b9/info.json)

You can enter your own IIIF image:

{{< rawhtml >}}
<form action="/" method="get">
  <input type="url" id="url" name="url" placeholder="URL info.json d'une image IIIF" style="width: 80%">
  <input type="submit" value="Voir">
</form>
{{< /rawhtml >}}

Or you can also try with one of the following images or those from the [exemples](/example/) page:

- __Atelier d'idéation d'Adno__ par les participants à la réunion du 23 juin  
[https://iiif.emf.fr/iiif/3/ideation.jpg/info.json](https://adno.app/?url=https://iiif.emf.fr/iiif/3/ideation.jpg/info.json) 
- __Voûte de l'abbaye de Saint-Savin__  
[https://iiif.emf.fr/iiif/3/saint-savin.jpg/info.json](/?url=https://iiif.emf.fr/iiif/3/saint-savin.jpg/info.json)
- __Tite-Live, Histoire romaine, version française par Pierre Bersuire__ Manuscrits de la Bibliothèque Sainte-Geneviève.    
[https://gallica.bnf.fr/iiif/ark:/12148/btv1b6001280q/f19/info.json](/?url=https://gallica.bnf.fr/iiif/ark:/12148/btv1b6001280q/f19/info.json)
- __Tapisserie de Bayeux__ Voir aussi [ici la version restaurée](https://www.bayeuxmuseum.com/la-tapisserie-de-bayeux/decouvrir-la-tapisserie-de-bayeux/explorer-la-tapisserie-de-bayeux-en-ligne/)  
[https://iiif.lib.ncsu.edu/iiif/xx-bayeux/info.json](/?url=https://iiif.lib.ncsu.edu/iiif/xx-bayeux/info.json)
- __Chat "regardant" à travers une longue-vue et autre chat perché dessus (Agence Rol)__ BnF, département Estampes et photographie, EST EI-13 (89).  
[https://gallica.bnf.fr/iiif/ark:/12148/btv1b69162903/f1/info.json](/?url=https://gallica.bnf.fr/iiif/ark:/12148/btv1b69162903/f1/info.json)
- __Un souvenir de vacances__ Une « planche de science » réalisée par Camille Arnoult du lycée Camille Jullian (Bordeaux).  
[https://iiif.emf.fr/iiif/3/UnSouvenirDeVacances.jp2/info.json](/?url=https://iiif.emf.fr/iiif/3/UnSouvenirDeVacances.jp2/info.json)

The previous images are provided by IIIF servers. However, it is also possible to do without and to provide a static IIF image made up of a info.json file and an arborescence of tiles. See this [tutorial](http://ronallo.com/iiif-workshop-new/image-api/image-servers/static.html).

- __Étoiles de mer__ Image statique IIIF. Voir la structure à [cette adresse](https://static.emf.fr/adno/static/iiif/starfish/)   
[https://static.emf.fr/adno/static/iiif/starfish/info.json](https://adno.app/?url=https://static.emf.fr/adno/static/iiif/starfish/info.json)

You can also use non-IIIF images:

- __Sonde Cassini__ DZI (Deep Zoom Image). Cf. structure [here](https://static.emf.fr/adno/static/dzi/)  
[https://static.emf.fr/dev/dzi/cassini.dzi](https://adno.app/?url=https://static.emf.fr/adno/static/dzi/cassini.dzi)
- __Mario__ image statique au format png  
[https://www.pngmart.com/files/2/Mario-PNG-Image.png](https://adno.app/?url=https://www.pngmart.com/files/2/Mario-PNG-Image.png)
- __Panorama de Poitiers__ image statique au format jpg (Lucas Aless)  
[https://upload.wikimedia.org/wikipedia/commons/1/1d/Poitiers_panorama_01.jpg](https://adno.app?url=https://upload.wikimedia.org/wikipedia/commons/1/1d/Poitiers_panorama_01.jpg)

## Adno is based on open source software

Adno uses existing open source components, including [OpenSeaDragon](https://openseadragon.github.io/) viewer and [Annotorious](https://recogito.github.io/annotorious/) to create annotations.

