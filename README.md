# Plan comptable formattée (version 2023)

Le plan comptable complet en **format JSON**.

La version est conforme à l'édition du **1er janvier 2023** du **RÈGLEMENT ANC N° 2014-03**.

<br/>
Le document prend la forme suivante: 
```js
[
  {
    "number": 1, // numéro de la classe
    "label": "Capitaux", // nom de la classe
    "accounts": [ // liste des comptes de la classe
      {
        "number": 21, // numéro du compte
        "label": "Capital et réserves", // nom du compte
        "accounts": [
          // les sous-comptes 21X, eux-mêmes ayant des sous-comptes suivant la même structure
          ...
        ]
      },
      ...
    ]
  },
  ...
]
```
