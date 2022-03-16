# Classes utilitaires d'espacement

Fonction SASS qui génère des class css utilitaires pour gérer l'espacement selon les différentes tailles d'écran.

## Usage

Nomenclature des class CSS

```
{propriété}-{breakpoint}-{valeur}

```

Par exemple, les class suivantes : 

```
<h1 class="mb-xs-2 mb-md-4">Contenu</h1>

```

applique la règle css suivante :

```
h1 {
    @media screen and (min-width: 0) {
        .mb-xs-2 {
            margin-bottom: 0.5rem;
        }
    }
    
    @media screen and (min-width: 768px) {
        .mb-md-4 {
            margin-bottom: 1.5rem;
        }
    }
 }  
    
```

## Propriétés

```
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

```

## Breakpoints

```
$breakpoints: (
    xs: 0,
    sm: 576px,
    md: 768px,
    lg: 1024px,
    xl: 1280px,
    xxl: 1920px,
) !default;

```

## Valeurs

```
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

```

