# Zenkai3D Studio - eines

Les eines internes de l'estudi. Son pagines d'una sola pagina, sense servidor:
funcionen al navegador i desen les dades al Google Drive del compte amb que
inicies sessio (zenkai3dstudio@gmail.com).

| Fitxer | Que es |
|---|---|
| `index.html` | El menu. Troba les eines ell sol preguntant la llista de fitxers a GitHub |
| `inventari.html` | Inventari de filament: bobines, colors, valor de l'estoc i que cal demanar |
| `pressupost.html` | Pressupost d'impressio, filament i resina, amb pintat i preu d'amic |
| `collabs.html` | Col·laboracions amb marques i concursos oberts |
| `impressions.html` | Registre d'impressions: llegeix el fitxer del slicer i descompta de l'inventari |
| `instagram.html` | Estadistiques: reels, abast, seguidors i visites al portfolio |
| `zenkai.js` | La porta d'entrada de Google i la capa del Drive, compartides |
| `zenkai-nav.js` | La barra de dalt que salta d'una eina a l'altra |
| `zenkai.css` | L'estil compartit |
| `icona.png` | El logo, un sol cop per a totes |

## Entrar-hi

Cada eina demana el compte de Google un cop i es queda la sessio una hora,
compartida entre totes perque son del mateix domini. El permis es `drive.file`:
nomes veuen els fitxers que han creat elles mateixes.

El Client ID d'OAuth s'escriu una vegada i es desa al navegador. **Es per
adreca**: en canviar de domini s'ha de tornar a escriure, i el domini nou s'ha
d'afegir als origens autoritzats del client d'OAuth a la Google Cloud Console,
o l'inici de sessio no funciona enlloc.

## Publicar

GitHub Pages des de l'arrel de `main`. El `.nojekyll` hi es perque Pages no
toqui res.

El portfolio public viu a part, al repositori `mediakit`: aquestes son eines
amb contrasenya i aquell es l'unic que es pot ensenyar.
