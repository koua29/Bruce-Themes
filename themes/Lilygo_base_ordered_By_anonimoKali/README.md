# Lilygo_base_ordered

Version **corrigée** du thème [`Lilygo_base_By_anonimoKali`](../Lilygo_base_By_anonimoKali) pour le firmware **Bruce** (LilyGO T-Embed CC1101 et autres).

## Ce qui change

Dans le thème d'origine, chaque icône est une « capture de carrousel » où les
menus **précédent** (en haut) et **suivant** (en bas) sont dessinés dans l'image.
Ces voisins étaient figés sur un ordre de menu différent de celui du firmware Bruce
actuel : à l'écran, les aperçus haut/bas ne correspondaient pas au menu réellement
atteint en tournant la molette (ex. RFID annonçait RF/IR au lieu de GPS/FILES).

Cette version **remappe les bandes haut/bas** de chaque icône pour qu'elles reflètent
l'ordre réel du menu (haut = précédent, bas = suivant) :

```
Config → Wifi → BLE → RF → NRF24 → LORA → FM → IR → ETH → GPS → RFID → FILES → JS → CLOCK → OTHERS → (Config)
```

Le logo central de chaque icône est **inchangé** ; seules les mini-étiquettes
voisines ont été corrigées. Fait pour les 4 résolutions (105 / 140 / 180 / 192 px).

## Installation

1. Copier le dossier de la taille correspondant à ton écran (T-Embed CC1101 = `140px`)
   dans `/themes/` de la carte SD.
2. Sur l'appareil : **Settings → Themes → `Theme_Lilygo_base_ordered.json`**.

## Crédits

- Thème original : **anonimoKali** — design et icônes.
- Correction de l'ordre des menus : **koua29**.
- Licence : **GNU GPLv3** (identique à l'original).
