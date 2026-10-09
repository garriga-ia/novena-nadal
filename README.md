# Novena de Nadal · Els nou dies

## Què hi ha al paquet

Hi ha nou carpetes, `dia-1` fins a `dia-9`. Cada carpeta inclou:

- `dia-N.html`: la pàgina del dia, amb el disseny publicat i les set imatges incrustades. No necessita biblioteques ni imatges externes.
- `audio-dia-N-1.mp3` fins a `audio-dia-N-6.mp3`: sis àudios substituïbles, al costat de l'HTML.
- `index.html`: obre automàticament `dia-N.html` quan entres a la carpeta.
- `.nojekyll`: fitxer buit per publicar els fitxers directament.

La lletra N representa el número del dia. Els punts 3 (lectura i reflexió) i 4 (peticions) només tenen àudio; els punts 1, 2, 5 i 6 tenen text i àudio. Tots mantenen el botó Escoltar i la il·lustració.

Els 54 MP3 inclosos són àudios de mostra amb veu sintètica masculina en català. Són provisionals: substituïu-los per les gravacions de la família. Aquesta nota és només al README, no a les pàgines de pregària.

## Penjar-ho a GitHub Pages des del navegador

1. Descarrega `novena-completa.zip` i descomprimeix-lo. No pugis el ZIP: puja les nou carpetes de dins i aquest README.
2. Obre el repositori de GitHub on vols publicar-ho.
3. A **Code**, tria **Add file > Upload files**. Arrossega les carpetes `dia-1` fins a `dia-9` al repositori conservant-ne l'estructura. Mantén cada HTML i els seus sis MP3 junts. Són 82 fitxers en total, per sota del límit de 100 per pujada. Si el navegador no mostra `.nojekyll`, pots afegir un fitxer buit amb aquest nom a l'arrel del repositori; aquestes pàgines HTML també es poden publicar sense ell.
4. Escriu un missatge com `Afegir els nou dies de la novena`, confirma la pujada i, si has creat una branca nova, completa el pull request i fusiona'l a la branca que publicaràs.
5. A **Settings > Pages**, a **Build and deployment**, tria **Deploy from a branch**. Selecciona la branca on has pujat els fitxers (normalment `main`) i la carpeta **/(root)**. Prem **Save**. Cal que el teu pla i la visibilitat del repositori permetin GitHub Pages.
6. Quan acabi la publicació, prem **Visit site** a **Settings > Pages** per obtenir l'adreça real. No és l'adreça de la vista del fitxer a github.com.
7. Des d'aquesta adreça base, obre `dia-1/`, `dia-2/` i així fins a `dia-9/`. Cada carpeta obre el seu dia automàticament. També pots obrir `dia-1/dia-1.html`, per exemple. El paquet no inclou un índex a l'arrel: publica i comparteix els enllaços de cada dia.

Si el repositori ja té un web, no sobreescriguis el seu `index.html` ni canviïs la configuració de Pages sense comprovar-la. Posa les nou carpetes dins de la carpeta que ja publica Pages. Si la font és `/docs`, posa-les allà.

## Penjar-ho amb Git

Dins d'un clon local del teu repositori, copia les nou carpetes i aquest README. Si el web ja té un README, conserva'l o copia aquest amb un altre nom. Després executa:

```sh
git add dia-1 dia-2 dia-3 dia-4 dia-5 dia-6 dia-7 dia-8 dia-9
git add README.md
git commit -m "Afegir els nou dies de la novena"
git push
```

Configura **Settings > Pages > Deploy from a branch** amb la branca i carpeta correctes, si no estava configurat.

## Posar-hi els vostres àudios

Grava o exporta àudio en format MP3 real. Canviar només l'extensió d'un M4A o OGG no el converteix a MP3.

| Fitxer dins de cada carpeta | Punt |
| --- | --- |
| `audio-dia-N-1.mp3` | Senyal de la creu |
| `audio-dia-N-2.mp3` | Pregària inicial |
| `audio-dia-N-3.mp3` | Lectura i reflexió del dia |
| `audio-dia-N-4.mp3` | Peticions |
| `audio-dia-N-5.mp3` | Parenostre, avemaria i glòria |
| `audio-dia-N-6.mp3` | Pregària final |

Exemple: la lectura del dia 4 és `dia-4/audio-dia-4-3.mp3`.

Substitueix els MP3 mantenint els noms exactes, en minúscules, i la mateixa carpeta. Amb el navegador, obre la carpeta del dia i tria **Add file > Upload files**. Amb Git, reemplaça els fitxers locals i confirma i puja els canvis. No cal tocar el reproductor de l'HTML. La pujada des del navegador admet fins a 25 MiB per fitxer: si una gravació és més grossa, exporta-la més comprimida o utilitza Git/GitHub Desktop.

## Comprovar que funciona

- Obre el web publicat amb **Visit site**, no l'HTML del repositori.
- Obre cada carpeta de dia i prova els sis botons Escoltar. El punt 4 no ha de mostrar les peticions escrites.
- Canvia de punt mentre sona: l'anterior s'ha d'aturar. Torna a tocar el botó per pausar.
- Si encara escoltes la gravació antiga després d'una substitució, espera que Pages acabi de publicar i torna a carregar la pàgina; prova una pestanya privada per descartar la memòria cau.
- Si un àudio falla, comprova que el nom del MP3 coincideix exactament i que és al mateix directori que l'HTML.

GitHub Pages publica el web a internet: comparteix només gravacions que tingueu permís per publicar. La prova d'escriptori no garanteix el funcionament dins del navegador integrat de WhatsApp: si falla allà, obre l'enllaç amb Safari o Chrome. Per preparar la pujada a GitHub, descarregar i descomprimir el ZIP a l'ordinador és el més còmode.

## Referències

- Pujada de fitxers: https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository
- Configuració de Pages: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
