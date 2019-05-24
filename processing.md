# Processing
Processing on työkalu, jolla saa tuotettua helposti visuaalista tulostetta pelkän tekstin sijaan
## Asennus
Asennus onnistuu raspberrylle komennolla
```
curl https://processing.org/download/install-arm.sh | sudo sh
```
Osoitteesta https://processing.org/download/ voi ladata myös macille, linuxille ja windowsille.

Ota käyttöön python-tila oikeasta yläkulmasta: Add mode.. -> Python mode for Processing 3 -> Install
Samassa ikkunassa valitse välilehti Libraries. Etsi ja asenna MQTT, niin saat yhdistettyä shiftr:iin.

## Ensimmäinen ohjelma

```
size(1024, 576)
line(100, 200, 400, 500)
```
Ohjelma luo ikkunan, jonka koko on 1024x576 ja piirtää suoran pisteestä (100, 200) pisteeseen (400, 500).

Viivan väriä saa vaihdettua funkiolla stroke ja paksuutta funktiolla strokeWeight
```
stroke("#ff0000")           # Punainen hex
stroke(255, 0, 0)           # Punainen RGB

strokeWidth(30)             # 30px paksu
```
Nämä vaikuttavat kaikkiin tuleviin piirroksiin, jos niitä ei vaihdeta välissä. Esimerkiksi seuraava koodi piirtää kaksi punaista viivaa:
```
stroke(255, 0, 0)
line(100, 100, 100, 200)
line(100, 100, 200, 100)
```

Muita piirtofunktioita:
```
point(300, 100)             # piste (x, y) koordinaatteihin
circle(200, 200, 50)        # ympyrä, ensin x, y -koordinaatit, sitten säde
ellipse(200, 200, 100, 50)  # ellipsi, ensin x, y -koordinaatit, sitten leveys ja korkeus



beginShape()                # piirtää monikulmion, jonka kulmat ovat pisteissä (300, 200), (300, 300) ja (400, 400)
vertex(300, 200)
vertex(300, 300)
vertex(400, 400)
endShape(CLOSE)


```
