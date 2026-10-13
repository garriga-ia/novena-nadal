# Novena de Nadal: els nou dies

Aquest paquet conté les nou pàgines de la novena, amb el text complet dels punts 3 (lectura i reflexió) i 4 (peticions). El disseny, les imatges i els textos corresponen a les versions publicades el 13 d'octubre de 2026.

## Contingut

Cada carpeta `dia-1` fins a `dia-9` conté:

- `dia-N.html`: la pàgina del dia, amb les imatges incrustades.
- `index.html`: obre automàticament `dia-N.html`.
- Sis arxius `audio-dia-N-1.mp3` fins a `audio-dia-N-6.mp3`.
- `.nojekyll`: evita el processament de Jekyll quan aquesta carpeta és l'arrel publicada.

Els botons "Escoltar" reprodueixen els MP3 de la mateixa carpeta. No necessiten cap servei de veu extern.

## Pujar-ho a GitHub Pages

1. Descomprimiu `novena-completa-v2.zip` a l'ordinador.
2. Obriu el repositori del vostre web a GitHub.
3. A la carpeta que publica GitHub Pages, feu servir **Add file > Upload files**. Si Pages publica des de `/docs`, pugeu-ho dins de `docs`; si publica des de l'arrel, pugeu-ho a l'arrel.
4. Arrossegueu les nou carpetes completes, mantenint-ne els noms i tots els fitxers interiors. No pugeu el ZIP sense descomprimir. Si ja hi ha versions anteriors, substituïu-ne els fitxers.
5. Comproveu que els fitxers ocults `.nojekyll` també s'han pujat. Per desactivar Jekyll a tot el web, podeu afegir un `.nojekyll` buit a l'arrel que publica Pages.
6. Feu **Commit changes**. Si encara no està activat, aneu a **Settings > Pages**, trieu **Deploy from a branch** i seleccioneu la branca i la carpeta correctes.
7. Quan GitHub indiqui que el desplegament ha acabat, obriu l'adreça del vostre web seguida de `/dia-1/`, `/dia-2/`, etc. També podeu obrir directament `/dia-1/dia-1.html`.
8. Reviseu cada dia i proveu els botons "Escoltar" des del mòbil.

## Substituir els àudios

Els MP3 inclosos són àudios sintètics provisionals. Aquesta nota només és al README, no a les pàgines.

Quan tingueu les gravacions definitives, substituïu cada MP3 mantenint exactament el mateix nom i la mateixa carpeta. No cal editar l'HTML.

Els números corresponen a:

1. Senyal de la creu
2. Pregària inicial
3. Lectura i reflexió del dia
4. Peticions
5. Parenostre, avemaria i glòria
6. Pregària final

Per exemple, la lectura del dia 3 ha de continuar dient-se `dia-3/audio-dia-3-3.mp3`. Feu un nou commit i espereu el desplegament de Pages. Si el navegador encara reprodueix l'àudio antic, actualitzeu la pàgina o buideu-ne la memòria cau.

## Prova a l'ordinador

Podeu obrir `dia-N.html` directament al navegador des de la carpeta descomprimida. Manteniu els sis MP3 al costat de l'HTML.

Recordeu que en un repositori públic i a GitHub Pages els arxius poden ser accessibles a qualsevol persona amb l'enllaç. Publiqueu només els àudios que vulgueu compartir.
