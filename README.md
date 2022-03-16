# Classes utilitaires d'espacement

Fonction SASS qui génère des class css utilitaires pour gérer l'espacement selon les différentes tailles d'écran.
## Nomenclature des class CSS

`{propriété}-{breakpoint}-{valeur}`

Cette Exemple : 

`<h1 class="mb-xs-2">Contenu</h1>`

applique la règle css suivante au <h1> :

`
    @media screen and (min-width: 0) {
        .mb-xs-2 {
            margin-bottom: 0.5rem;
        }
    }
`

## Propriétés

`
    p:  padding,
    pt: padding-top,
    pr: padding-right,
    pb: padding-bottom,
    pl: padding-left,
    m:  margin,
    mt: margin-top,
    mr: margin-right,
    mb: margin-bottom,
    ml: margin-left,

`

## Breakpoints

`
p:  padding,
pt: padding-top,
pr: padding-right,
pb: padding-bottom,
pl: padding-left,
m:  margin,
mt: margin-top,
mr: margin-right,
mb: margin-bottom,
ml: margin-left,

`

## Valeurs

`
$spacer: 1 !default; //1rem
$spacers: () !default;
$spacers: map-merge((
    0: 0,
    1: ($spacer * .25),  //4px
    2: ($spacer * .5),   //8px
    3: $spacer,         //16px
    4: ($spacer * 1.5), //24px
    5: ($spacer * 3),   //48px
    6: ($spacer * 4),   //64px
    7: ($spacer * 6),   //96px
    ),
$spacers);

`
