# tounsi-invest-data

Données réelles de la Bourse de Tunis (BVMT) utilisées par l'application **Tounsi Invest**.

## Contenu — `latest.json`

- `tunindex` : historique quotidien du TUNINDEX (2015-07 → aujourd'hui)
- `stocks` : 10 valeurs tunisiennes (SFBT, BT, AB, ATB, BIAT, BNA, PGH, OTH, DH, SOTET), historique quotidien depuis 2016-07

Format compact : pour chaque série, `d` = dates ISO, `c` = clôtures, `v` = volumes (tableaux alignés).

## Sources

- TUNINDEX : african-markets.com (recoupé avec les performances annuelles officielles BVMT)
- Valeurs : ilboursa.com

Consommation : l'app récupère `https://raw.githubusercontent.com/uzushitn/tounsi-invest-data/main/latest.json` et fusionne les points plus récents dans sa base locale.