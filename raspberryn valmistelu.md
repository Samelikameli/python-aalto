## Levynkuvan lataaminen ja poltto
1. Lataa levynkuva osoitteesta https://github.com/google/aiyprojects-raspbian/releases ja valitse uusin
2. Polta kuva SD-kortille esimerkiksi Etcherillä tai dd:llä

## Raspberryn käynnistys
1. Kytke hdmi-kaapeli, näppäimistö, hiiri ja virtalähde ja odota, kunnes raspberry käynnistyy
2. Ensimmäisen käynnistyksen jälkeen tulee ikkuna, jolla voi valita olennaisia asetuksia. Valitse ensimmäisessä näkymässä Next
3. Jos haluat kieleksi englannin, valitse sijainniksi United Kingdom ja kieleksi British English. Jos haluat suomen, valitse sijainniksi Finland ja kieleksi Finnish.
4. Poista valinta kohdasta "Use US keyboard" ja paina Next
5. Valitse Next ilman, että vaihdat salasanaa
6. Yhdistä wifiin
7. Hyväksy ohjelmistopäivitys ja odota sen valmistuminen
8. Kun päivitys on valmis, valitse ok ja reboot.
9. Vaihda näppäimistöasettelu ja aikavyöhyke:

Varmista, että ainakin seuraavat ovat valittuina:

![](https://raw.githubusercontent.com/Samelikameli/python-aalto/master/guides/images/interfaces.png)

![](https://raw.githubusercontent.com/Samelikameli/python-aalto/master/guides/images/configuration.png)

![](https://raw.githubusercontent.com/Samelikameli/python-aalto/master/guides/images/localisation.png)

Aikavyöhykkeeksi Helsinki ja asetteluksi Finnish ja variantiksi Finnish.

## Asennus

1. Avaa terminaali näppäinyhdistelmällä Control+Alt+T
2. Asenna tarpeellisia python-kirjastoja komennolla 
```
sudo pip3 install flask paho-mqtt SpeechRecognition google-speech picamera 
```
3. Lataa paketti projekteja raspberrylle:
```
git clone https://github.com/Pohjois-Tapiolan-lukio/raspberry_pi-projects.git
```

## Google assistant
1. 
