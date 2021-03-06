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
## Class générés
```
@media screen and (min-width: 0) {
    .p-xs-0 {
      padding: 0rem;
    }
  
    .p-xs-1 {
      padding: 0.25rem;
    }
  
    .p-xs-2 {
      padding: 0.5rem;
    }
  
    .p-xs-3 {
      padding: 1rem;
    }
  
    .p-xs-4 {
      padding: 1.5rem;
    }
  
    .p-xs-5 {
      padding: 3rem;
    }
  
    .p-xs-6 {
      padding: 4rem;
    }
  
    .p-xs-7 {
      padding: 6rem;
    }
  
    .pt-xs-0 {
      padding-top: 0rem;
    }
  
    .pt-xs-1 {
      padding-top: 0.25rem;
    }
  
    .pt-xs-2 {
      padding-top: 0.5rem;
    }
  
    .pt-xs-3 {
      padding-top: 1rem;
    }
  
    .pt-xs-4 {
      padding-top: 1.5rem;
    }
  
    .pt-xs-5 {
      padding-top: 3rem;
    }
  
    .pt-xs-6 {
      padding-top: 4rem;
    }
  
    .pt-xs-7 {
      padding-top: 6rem;
    }
  
    .pr-xs-0 {
      padding-right: 0rem;
    }
  
    .pr-xs-1 {
      padding-right: 0.25rem;
    }
  
    .pr-xs-2 {
      padding-right: 0.5rem;
    }
  
    .pr-xs-3 {
      padding-right: 1rem;
    }
  
    .pr-xs-4 {
      padding-right: 1.5rem;
    }
  
    .pr-xs-5 {
      padding-right: 3rem;
    }
  
    .pr-xs-6 {
      padding-right: 4rem;
    }
  
    .pr-xs-7 {
      padding-right: 6rem;
    }
  
    .pb-xs-0 {
      padding-bottom: 0rem;
    }
  
    .pb-xs-1 {
      padding-bottom: 0.25rem;
    }
  
    .pb-xs-2 {
      padding-bottom: 0.5rem;
    }
  
    .pb-xs-3 {
      padding-bottom: 1rem;
    }
  
    .pb-xs-4 {
      padding-bottom: 1.5rem;
    }
  
    .pb-xs-5 {
      padding-bottom: 3rem;
    }
  
    .pb-xs-6 {
      padding-bottom: 4rem;
    }
  
    .pb-xs-7 {
      padding-bottom: 6rem;
    }
  
    .pl-xs-0 {
      padding-left: 0rem;
    }
  
    .pl-xs-1 {
      padding-left: 0.25rem;
    }
  
    .pl-xs-2 {
      padding-left: 0.5rem;
    }
  
    .pl-xs-3 {
      padding-left: 1rem;
    }
  
    .pl-xs-4 {
      padding-left: 1.5rem;
    }
  
    .pl-xs-5 {
      padding-left: 3rem;
    }
  
    .pl-xs-6 {
      padding-left: 4rem;
    }
  
    .pl-xs-7 {
      padding-left: 6rem;
    }
  
    .m-xs-0 {
      margin: 0rem;
    }
  
    .m-xs-1 {
      margin: 0.25rem;
    }
  
    .m-xs-2 {
      margin: 0.5rem;
    }
  
    .m-xs-3 {
      margin: 1rem;
    }
  
    .m-xs-4 {
      margin: 1.5rem;
    }
  
    .m-xs-5 {
      margin: 3rem;
    }
  
    .m-xs-6 {
      margin: 4rem;
    }
  
    .m-xs-7 {
      margin: 6rem;
    }
  
    .mt-xs-0 {
      margin-top: 0rem;
    }
  
    .mt-xs-1 {
      margin-top: 0.25rem;
    }
  
    .mt-xs-2 {
      margin-top: 0.5rem;
    }
  
    .mt-xs-3 {
      margin-top: 1rem;
    }
  
    .mt-xs-4 {
      margin-top: 1.5rem;
    }
  
    .mt-xs-5 {
      margin-top: 3rem;
    }
  
    .mt-xs-6 {
      margin-top: 4rem;
    }
  
    .mt-xs-7 {
      margin-top: 6rem;
    }
  
    .mr-xs-0 {
      margin-right: 0rem;
    }
  
    .mr-xs-1 {
      margin-right: 0.25rem;
    }
  
    .mr-xs-2 {
      margin-right: 0.5rem;
    }
  
    .mr-xs-3 {
      margin-right: 1rem;
    }
  
    .mr-xs-4 {
      margin-right: 1.5rem;
    }
  
    .mr-xs-5 {
      margin-right: 3rem;
    }
  
    .mr-xs-6 {
      margin-right: 4rem;
    }
  
    .mr-xs-7 {
      margin-right: 6rem;
    }
  
    .mb-xs-0 {
      margin-bottom: 0rem;
    }
  
    .mb-xs-1 {
      margin-bottom: 0.25rem;
    }
  
    .mb-xs-2 {
      margin-bottom: 0.5rem;
    }
  
    .mb-xs-3 {
      margin-bottom: 1rem;
    }
  
    .mb-xs-4 {
      margin-bottom: 1.5rem;
    }
  
    .mb-xs-5 {
      margin-bottom: 3rem;
    }
  
    .mb-xs-6 {
      margin-bottom: 4rem;
    }
  
    .mb-xs-7 {
      margin-bottom: 6rem;
    }
  
    .ml-xs-0 {
      margin-left: 0rem;
    }
  
    .ml-xs-1 {
      margin-left: 0.25rem;
    }
  
    .ml-xs-2 {
      margin-left: 0.5rem;
    }
  
    .ml-xs-3 {
      margin-left: 1rem;
    }
  
    .ml-xs-4 {
      margin-left: 1.5rem;
    }
  
    .ml-xs-5 {
      margin-left: 3rem;
    }
  
    .ml-xs-6 {
      margin-left: 4rem;
    }
  
    .ml-xs-7 {
      margin-left: 6rem;
    }
  }
  @media screen and (min-width: 576px) {
    .p-sm-0 {
      padding: 0rem;
    }
  
    .p-sm-1 {
      padding: 0.25rem;
    }
  
    .p-sm-2 {
      padding: 0.5rem;
    }
  
    .p-sm-3 {
      padding: 1rem;
    }
  
    .p-sm-4 {
      padding: 1.5rem;
    }
  
    .p-sm-5 {
      padding: 3rem;
    }
  
    .p-sm-6 {
      padding: 4rem;
    }
  
    .p-sm-7 {
      padding: 6rem;
    }
  
    .pt-sm-0 {
      padding-top: 0rem;
    }
  
    .pt-sm-1 {
      padding-top: 0.25rem;
    }
  
    .pt-sm-2 {
      padding-top: 0.5rem;
    }
  
    .pt-sm-3 {
      padding-top: 1rem;
    }
  
    .pt-sm-4 {
      padding-top: 1.5rem;
    }
  
    .pt-sm-5 {
      padding-top: 3rem;
    }
  
    .pt-sm-6 {
      padding-top: 4rem;
    }
  
    .pt-sm-7 {
      padding-top: 6rem;
    }
  
    .pr-sm-0 {
      padding-right: 0rem;
    }
  
    .pr-sm-1 {
      padding-right: 0.25rem;
    }
  
    .pr-sm-2 {
      padding-right: 0.5rem;
    }
  
    .pr-sm-3 {
      padding-right: 1rem;
    }
  
    .pr-sm-4 {
      padding-right: 1.5rem;
    }
  
    .pr-sm-5 {
      padding-right: 3rem;
    }
  
    .pr-sm-6 {
      padding-right: 4rem;
    }
  
    .pr-sm-7 {
      padding-right: 6rem;
    }
  
    .pb-sm-0 {
      padding-bottom: 0rem;
    }
  
    .pb-sm-1 {
      padding-bottom: 0.25rem;
    }
  
    .pb-sm-2 {
      padding-bottom: 0.5rem;
    }
  
    .pb-sm-3 {
      padding-bottom: 1rem;
    }
  
    .pb-sm-4 {
      padding-bottom: 1.5rem;
    }
  
    .pb-sm-5 {
      padding-bottom: 3rem;
    }
  
    .pb-sm-6 {
      padding-bottom: 4rem;
    }
  
    .pb-sm-7 {
      padding-bottom: 6rem;
    }
  
    .pl-sm-0 {
      padding-left: 0rem;
    }
  
    .pl-sm-1 {
      padding-left: 0.25rem;
    }
  
    .pl-sm-2 {
      padding-left: 0.5rem;
    }
  
    .pl-sm-3 {
      padding-left: 1rem;
    }
  
    .pl-sm-4 {
      padding-left: 1.5rem;
    }
  
    .pl-sm-5 {
      padding-left: 3rem;
    }
  
    .pl-sm-6 {
      padding-left: 4rem;
    }
  
    .pl-sm-7 {
      padding-left: 6rem;
    }
  
    .m-sm-0 {
      margin: 0rem;
    }
  
    .m-sm-1 {
      margin: 0.25rem;
    }
  
    .m-sm-2 {
      margin: 0.5rem;
    }
  
    .m-sm-3 {
      margin: 1rem;
    }
  
    .m-sm-4 {
      margin: 1.5rem;
    }
  
    .m-sm-5 {
      margin: 3rem;
    }
  
    .m-sm-6 {
      margin: 4rem;
    }
  
    .m-sm-7 {
      margin: 6rem;
    }
  
    .mt-sm-0 {
      margin-top: 0rem;
    }
  
    .mt-sm-1 {
      margin-top: 0.25rem;
    }
  
    .mt-sm-2 {
      margin-top: 0.5rem;
    }
  
    .mt-sm-3 {
      margin-top: 1rem;
    }
  
    .mt-sm-4 {
      margin-top: 1.5rem;
    }
  
    .mt-sm-5 {
      margin-top: 3rem;
    }
  
    .mt-sm-6 {
      margin-top: 4rem;
    }
  
    .mt-sm-7 {
      margin-top: 6rem;
    }
  
    .mr-sm-0 {
      margin-right: 0rem;
    }
  
    .mr-sm-1 {
      margin-right: 0.25rem;
    }
  
    .mr-sm-2 {
      margin-right: 0.5rem;
    }
  
    .mr-sm-3 {
      margin-right: 1rem;
    }
  
    .mr-sm-4 {
      margin-right: 1.5rem;
    }
  
    .mr-sm-5 {
      margin-right: 3rem;
    }
  
    .mr-sm-6 {
      margin-right: 4rem;
    }
  
    .mr-sm-7 {
      margin-right: 6rem;
    }
  
    .mb-sm-0 {
      margin-bottom: 0rem;
    }
  
    .mb-sm-1 {
      margin-bottom: 0.25rem;
    }
  
    .mb-sm-2 {
      margin-bottom: 0.5rem;
    }
  
    .mb-sm-3 {
      margin-bottom: 1rem;
    }
  
    .mb-sm-4 {
      margin-bottom: 1.5rem;
    }
  
    .mb-sm-5 {
      margin-bottom: 3rem;
    }
  
    .mb-sm-6 {
      margin-bottom: 4rem;
    }
  
    .mb-sm-7 {
      margin-bottom: 6rem;
    }
  
    .ml-sm-0 {
      margin-left: 0rem;
    }
  
    .ml-sm-1 {
      margin-left: 0.25rem;
    }
  
    .ml-sm-2 {
      margin-left: 0.5rem;
    }
  
    .ml-sm-3 {
      margin-left: 1rem;
    }
  
    .ml-sm-4 {
      margin-left: 1.5rem;
    }
  
    .ml-sm-5 {
      margin-left: 3rem;
    }
  
    .ml-sm-6 {
      margin-left: 4rem;
    }
  
    .ml-sm-7 {
      margin-left: 6rem;
    }
  }
  @media screen and (min-width: 768px) {
    .p-md-0 {
      padding: 0rem;
    }
  
    .p-md-1 {
      padding: 0.25rem;
    }
  
    .p-md-2 {
      padding: 0.5rem;
    }
  
    .p-md-3 {
      padding: 1rem;
    }
  
    .p-md-4 {
      padding: 1.5rem;
    }
  
    .p-md-5 {
      padding: 3rem;
    }
  
    .p-md-6 {
      padding: 4rem;
    }
  
    .p-md-7 {
      padding: 6rem;
    }
  
    .pt-md-0 {
      padding-top: 0rem;
    }
  
    .pt-md-1 {
      padding-top: 0.25rem;
    }
  
    .pt-md-2 {
      padding-top: 0.5rem;
    }
  
    .pt-md-3 {
      padding-top: 1rem;
    }
  
    .pt-md-4 {
      padding-top: 1.5rem;
    }
  
    .pt-md-5 {
      padding-top: 3rem;
    }
  
    .pt-md-6 {
      padding-top: 4rem;
    }
  
    .pt-md-7 {
      padding-top: 6rem;
    }
  
    .pr-md-0 {
      padding-right: 0rem;
    }
  
    .pr-md-1 {
      padding-right: 0.25rem;
    }
  
    .pr-md-2 {
      padding-right: 0.5rem;
    }
  
    .pr-md-3 {
      padding-right: 1rem;
    }
  
    .pr-md-4 {
      padding-right: 1.5rem;
    }
  
    .pr-md-5 {
      padding-right: 3rem;
    }
  
    .pr-md-6 {
      padding-right: 4rem;
    }
  
    .pr-md-7 {
      padding-right: 6rem;
    }
  
    .pb-md-0 {
      padding-bottom: 0rem;
    }
  
    .pb-md-1 {
      padding-bottom: 0.25rem;
    }
  
    .pb-md-2 {
      padding-bottom: 0.5rem;
    }
  
    .pb-md-3 {
      padding-bottom: 1rem;
    }
  
    .pb-md-4 {
      padding-bottom: 1.5rem;
    }
  
    .pb-md-5 {
      padding-bottom: 3rem;
    }
  
    .pb-md-6 {
      padding-bottom: 4rem;
    }
  
    .pb-md-7 {
      padding-bottom: 6rem;
    }
  
    .pl-md-0 {
      padding-left: 0rem;
    }
  
    .pl-md-1 {
      padding-left: 0.25rem;
    }
  
    .pl-md-2 {
      padding-left: 0.5rem;
    }
  
    .pl-md-3 {
      padding-left: 1rem;
    }
  
    .pl-md-4 {
      padding-left: 1.5rem;
    }
  
    .pl-md-5 {
      padding-left: 3rem;
    }
  
    .pl-md-6 {
      padding-left: 4rem;
    }
  
    .pl-md-7 {
      padding-left: 6rem;
    }
  
    .m-md-0 {
      margin: 0rem;
    }
  
    .m-md-1 {
      margin: 0.25rem;
    }
  
    .m-md-2 {
      margin: 0.5rem;
    }
  
    .m-md-3 {
      margin: 1rem;
    }
  
    .m-md-4 {
      margin: 1.5rem;
    }
  
    .m-md-5 {
      margin: 3rem;
    }
  
    .m-md-6 {
      margin: 4rem;
    }
  
    .m-md-7 {
      margin: 6rem;
    }
  
    .mt-md-0 {
      margin-top: 0rem;
    }
  
    .mt-md-1 {
      margin-top: 0.25rem;
    }
  
    .mt-md-2 {
      margin-top: 0.5rem;
    }
  
    .mt-md-3 {
      margin-top: 1rem;
    }
  
    .mt-md-4 {
      margin-top: 1.5rem;
    }
  
    .mt-md-5 {
      margin-top: 3rem;
    }
  
    .mt-md-6 {
      margin-top: 4rem;
    }
  
    .mt-md-7 {
      margin-top: 6rem;
    }
  
    .mr-md-0 {
      margin-right: 0rem;
    }
  
    .mr-md-1 {
      margin-right: 0.25rem;
    }
  
    .mr-md-2 {
      margin-right: 0.5rem;
    }
  
    .mr-md-3 {
      margin-right: 1rem;
    }
  
    .mr-md-4 {
      margin-right: 1.5rem;
    }
  
    .mr-md-5 {
      margin-right: 3rem;
    }
  
    .mr-md-6 {
      margin-right: 4rem;
    }
  
    .mr-md-7 {
      margin-right: 6rem;
    }
  
    .mb-md-0 {
      margin-bottom: 0rem;
    }
  
    .mb-md-1 {
      margin-bottom: 0.25rem;
    }
  
    .mb-md-2 {
      margin-bottom: 0.5rem;
    }
  
    .mb-md-3 {
      margin-bottom: 1rem;
    }
  
    .mb-md-4 {
      margin-bottom: 1.5rem;
    }
  
    .mb-md-5 {
      margin-bottom: 3rem;
    }
  
    .mb-md-6 {
      margin-bottom: 4rem;
    }
  
    .mb-md-7 {
      margin-bottom: 6rem;
    }
  
    .ml-md-0 {
      margin-left: 0rem;
    }
  
    .ml-md-1 {
      margin-left: 0.25rem;
    }
  
    .ml-md-2 {
      margin-left: 0.5rem;
    }
  
    .ml-md-3 {
      margin-left: 1rem;
    }
  
    .ml-md-4 {
      margin-left: 1.5rem;
    }
  
    .ml-md-5 {
      margin-left: 3rem;
    }
  
    .ml-md-6 {
      margin-left: 4rem;
    }
  
    .ml-md-7 {
      margin-left: 6rem;
    }
  }
  @media screen and (min-width: 1024px) {
    .p-lg-0 {
      padding: 0rem;
    }
  
    .p-lg-1 {
      padding: 0.25rem;
    }
  
    .p-lg-2 {
      padding: 0.5rem;
    }
  
    .p-lg-3 {
      padding: 1rem;
    }
  
    .p-lg-4 {
      padding: 1.5rem;
    }
  
    .p-lg-5 {
      padding: 3rem;
    }
  
    .p-lg-6 {
      padding: 4rem;
    }
  
    .p-lg-7 {
      padding: 6rem;
    }
  
    .pt-lg-0 {
      padding-top: 0rem;
    }
  
    .pt-lg-1 {
      padding-top: 0.25rem;
    }
  
    .pt-lg-2 {
      padding-top: 0.5rem;
    }
  
    .pt-lg-3 {
      padding-top: 1rem;
    }
  
    .pt-lg-4 {
      padding-top: 1.5rem;
    }
  
    .pt-lg-5 {
      padding-top: 3rem;
    }
  
    .pt-lg-6 {
      padding-top: 4rem;
    }
  
    .pt-lg-7 {
      padding-top: 6rem;
    }
  
    .pr-lg-0 {
      padding-right: 0rem;
    }
  
    .pr-lg-1 {
      padding-right: 0.25rem;
    }
  
    .pr-lg-2 {
      padding-right: 0.5rem;
    }
  
    .pr-lg-3 {
      padding-right: 1rem;
    }
  
    .pr-lg-4 {
      padding-right: 1.5rem;
    }
  
    .pr-lg-5 {
      padding-right: 3rem;
    }
  
    .pr-lg-6 {
      padding-right: 4rem;
    }
  
    .pr-lg-7 {
      padding-right: 6rem;
    }
  
    .pb-lg-0 {
      padding-bottom: 0rem;
    }
  
    .pb-lg-1 {
      padding-bottom: 0.25rem;
    }
  
    .pb-lg-2 {
      padding-bottom: 0.5rem;
    }
  
    .pb-lg-3 {
      padding-bottom: 1rem;
    }
  
    .pb-lg-4 {
      padding-bottom: 1.5rem;
    }
  
    .pb-lg-5 {
      padding-bottom: 3rem;
    }
  
    .pb-lg-6 {
      padding-bottom: 4rem;
    }
  
    .pb-lg-7 {
      padding-bottom: 6rem;
    }
  
    .pl-lg-0 {
      padding-left: 0rem;
    }
  
    .pl-lg-1 {
      padding-left: 0.25rem;
    }
  
    .pl-lg-2 {
      padding-left: 0.5rem;
    }
  
    .pl-lg-3 {
      padding-left: 1rem;
    }
  
    .pl-lg-4 {
      padding-left: 1.5rem;
    }
  
    .pl-lg-5 {
      padding-left: 3rem;
    }
  
    .pl-lg-6 {
      padding-left: 4rem;
    }
  
    .pl-lg-7 {
      padding-left: 6rem;
    }
  
    .m-lg-0 {
      margin: 0rem;
    }
  
    .m-lg-1 {
      margin: 0.25rem;
    }
  
    .m-lg-2 {
      margin: 0.5rem;
    }
  
    .m-lg-3 {
      margin: 1rem;
    }
  
    .m-lg-4 {
      margin: 1.5rem;
    }
  
    .m-lg-5 {
      margin: 3rem;
    }
  
    .m-lg-6 {
      margin: 4rem;
    }
  
    .m-lg-7 {
      margin: 6rem;
    }
  
    .mt-lg-0 {
      margin-top: 0rem;
    }
  
    .mt-lg-1 {
      margin-top: 0.25rem;
    }
  
    .mt-lg-2 {
      margin-top: 0.5rem;
    }
  
    .mt-lg-3 {
      margin-top: 1rem;
    }
  
    .mt-lg-4 {
      margin-top: 1.5rem;
    }
  
    .mt-lg-5 {
      margin-top: 3rem;
    }
  
    .mt-lg-6 {
      margin-top: 4rem;
    }
  
    .mt-lg-7 {
      margin-top: 6rem;
    }
  
    .mr-lg-0 {
      margin-right: 0rem;
    }
  
    .mr-lg-1 {
      margin-right: 0.25rem;
    }
  
    .mr-lg-2 {
      margin-right: 0.5rem;
    }
  
    .mr-lg-3 {
      margin-right: 1rem;
    }
  
    .mr-lg-4 {
      margin-right: 1.5rem;
    }
  
    .mr-lg-5 {
      margin-right: 3rem;
    }
  
    .mr-lg-6 {
      margin-right: 4rem;
    }
  
    .mr-lg-7 {
      margin-right: 6rem;
    }
  
    .mb-lg-0 {
      margin-bottom: 0rem;
    }
  
    .mb-lg-1 {
      margin-bottom: 0.25rem;
    }
  
    .mb-lg-2 {
      margin-bottom: 0.5rem;
    }
  
    .mb-lg-3 {
      margin-bottom: 1rem;
    }
  
    .mb-lg-4 {
      margin-bottom: 1.5rem;
    }
  
    .mb-lg-5 {
      margin-bottom: 3rem;
    }
  
    .mb-lg-6 {
      margin-bottom: 4rem;
    }
  
    .mb-lg-7 {
      margin-bottom: 6rem;
    }
  
    .ml-lg-0 {
      margin-left: 0rem;
    }
  
    .ml-lg-1 {
      margin-left: 0.25rem;
    }
  
    .ml-lg-2 {
      margin-left: 0.5rem;
    }
  
    .ml-lg-3 {
      margin-left: 1rem;
    }
  
    .ml-lg-4 {
      margin-left: 1.5rem;
    }
  
    .ml-lg-5 {
      margin-left: 3rem;
    }
  
    .ml-lg-6 {
      margin-left: 4rem;
    }
  
    .ml-lg-7 {
      margin-left: 6rem;
    }
  }
  @media screen and (min-width: 1280px) {
    .p-xl-0 {
      padding: 0rem;
    }
  
    .p-xl-1 {
      padding: 0.25rem;
    }
  
    .p-xl-2 {
      padding: 0.5rem;
    }
  
    .p-xl-3 {
      padding: 1rem;
    }
  
    .p-xl-4 {
      padding: 1.5rem;
    }
  
    .p-xl-5 {
      padding: 3rem;
    }
  
    .p-xl-6 {
      padding: 4rem;
    }
  
    .p-xl-7 {
      padding: 6rem;
    }
  
    .pt-xl-0 {
      padding-top: 0rem;
    }
  
    .pt-xl-1 {
      padding-top: 0.25rem;
    }
  
    .pt-xl-2 {
      padding-top: 0.5rem;
    }
  
    .pt-xl-3 {
      padding-top: 1rem;
    }
  
    .pt-xl-4 {
      padding-top: 1.5rem;
    }
  
    .pt-xl-5 {
      padding-top: 3rem;
    }
  
    .pt-xl-6 {
      padding-top: 4rem;
    }
  
    .pt-xl-7 {
      padding-top: 6rem;
    }
  
    .pr-xl-0 {
      padding-right: 0rem;
    }
  
    .pr-xl-1 {
      padding-right: 0.25rem;
    }
  
    .pr-xl-2 {
      padding-right: 0.5rem;
    }
  
    .pr-xl-3 {
      padding-right: 1rem;
    }
  
    .pr-xl-4 {
      padding-right: 1.5rem;
    }
  
    .pr-xl-5 {
      padding-right: 3rem;
    }
  
    .pr-xl-6 {
      padding-right: 4rem;
    }
  
    .pr-xl-7 {
      padding-right: 6rem;
    }
  
    .pb-xl-0 {
      padding-bottom: 0rem;
    }
  
    .pb-xl-1 {
      padding-bottom: 0.25rem;
    }
  
    .pb-xl-2 {
      padding-bottom: 0.5rem;
    }
  
    .pb-xl-3 {
      padding-bottom: 1rem;
    }
  
    .pb-xl-4 {
      padding-bottom: 1.5rem;
    }
  
    .pb-xl-5 {
      padding-bottom: 3rem;
    }
  
    .pb-xl-6 {
      padding-bottom: 4rem;
    }
  
    .pb-xl-7 {
      padding-bottom: 6rem;
    }
  
    .pl-xl-0 {
      padding-left: 0rem;
    }
  
    .pl-xl-1 {
      padding-left: 0.25rem;
    }
  
    .pl-xl-2 {
      padding-left: 0.5rem;
    }
  
    .pl-xl-3 {
      padding-left: 1rem;
    }
  
    .pl-xl-4 {
      padding-left: 1.5rem;
    }
  
    .pl-xl-5 {
      padding-left: 3rem;
    }
  
    .pl-xl-6 {
      padding-left: 4rem;
    }
  
    .pl-xl-7 {
      padding-left: 6rem;
    }
  
    .m-xl-0 {
      margin: 0rem;
    }
  
    .m-xl-1 {
      margin: 0.25rem;
    }
  
    .m-xl-2 {
      margin: 0.5rem;
    }
  
    .m-xl-3 {
      margin: 1rem;
    }
  
    .m-xl-4 {
      margin: 1.5rem;
    }
  
    .m-xl-5 {
      margin: 3rem;
    }
  
    .m-xl-6 {
      margin: 4rem;
    }
  
    .m-xl-7 {
      margin: 6rem;
    }
  
    .mt-xl-0 {
      margin-top: 0rem;
    }
  
    .mt-xl-1 {
      margin-top: 0.25rem;
    }
  
    .mt-xl-2 {
      margin-top: 0.5rem;
    }
  
    .mt-xl-3 {
      margin-top: 1rem;
    }
  
    .mt-xl-4 {
      margin-top: 1.5rem;
    }
  
    .mt-xl-5 {
      margin-top: 3rem;
    }
  
    .mt-xl-6 {
      margin-top: 4rem;
    }
  
    .mt-xl-7 {
      margin-top: 6rem;
    }
  
    .mr-xl-0 {
      margin-right: 0rem;
    }
  
    .mr-xl-1 {
      margin-right: 0.25rem;
    }
  
    .mr-xl-2 {
      margin-right: 0.5rem;
    }
  
    .mr-xl-3 {
      margin-right: 1rem;
    }
  
    .mr-xl-4 {
      margin-right: 1.5rem;
    }
  
    .mr-xl-5 {
      margin-right: 3rem;
    }
  
    .mr-xl-6 {
      margin-right: 4rem;
    }
  
    .mr-xl-7 {
      margin-right: 6rem;
    }
  
    .mb-xl-0 {
      margin-bottom: 0rem;
    }
  
    .mb-xl-1 {
      margin-bottom: 0.25rem;
    }
  
    .mb-xl-2 {
      margin-bottom: 0.5rem;
    }
  
    .mb-xl-3 {
      margin-bottom: 1rem;
    }
  
    .mb-xl-4 {
      margin-bottom: 1.5rem;
    }
  
    .mb-xl-5 {
      margin-bottom: 3rem;
    }
  
    .mb-xl-6 {
      margin-bottom: 4rem;
    }
  
    .mb-xl-7 {
      margin-bottom: 6rem;
    }
  
    .ml-xl-0 {
      margin-left: 0rem;
    }
  
    .ml-xl-1 {
      margin-left: 0.25rem;
    }
  
    .ml-xl-2 {
      margin-left: 0.5rem;
    }
  
    .ml-xl-3 {
      margin-left: 1rem;
    }
  
    .ml-xl-4 {
      margin-left: 1.5rem;
    }
  
    .ml-xl-5 {
      margin-left: 3rem;
    }
  
    .ml-xl-6 {
      margin-left: 4rem;
    }
  
    .ml-xl-7 {
      margin-left: 6rem;
    }
  }
  @media screen and (min-width: 1920px) {
    .p-xxl-0 {
      padding: 0rem;
    }
  
    .p-xxl-1 {
      padding: 0.25rem;
    }
  
    .p-xxl-2 {
      padding: 0.5rem;
    }
  
    .p-xxl-3 {
      padding: 1rem;
    }
  
    .p-xxl-4 {
      padding: 1.5rem;
    }
  
    .p-xxl-5 {
      padding: 3rem;
    }
  
    .p-xxl-6 {
      padding: 4rem;
    }
  
    .p-xxl-7 {
      padding: 6rem;
    }
  
    .pt-xxl-0 {
      padding-top: 0rem;
    }
  
    .pt-xxl-1 {
      padding-top: 0.25rem;
    }
  
    .pt-xxl-2 {
      padding-top: 0.5rem;
    }
  
    .pt-xxl-3 {
      padding-top: 1rem;
    }
  
    .pt-xxl-4 {
      padding-top: 1.5rem;
    }
  
    .pt-xxl-5 {
      padding-top: 3rem;
    }
  
    .pt-xxl-6 {
      padding-top: 4rem;
    }
  
    .pt-xxl-7 {
      padding-top: 6rem;
    }
  
    .pr-xxl-0 {
      padding-right: 0rem;
    }
  
    .pr-xxl-1 {
      padding-right: 0.25rem;
    }
  
    .pr-xxl-2 {
      padding-right: 0.5rem;
    }
  
    .pr-xxl-3 {
      padding-right: 1rem;
    }
  
    .pr-xxl-4 {
      padding-right: 1.5rem;
    }
  
    .pr-xxl-5 {
      padding-right: 3rem;
    }
  
    .pr-xxl-6 {
      padding-right: 4rem;
    }
  
    .pr-xxl-7 {
      padding-right: 6rem;
    }
  
    .pb-xxl-0 {
      padding-bottom: 0rem;
    }
  
    .pb-xxl-1 {
      padding-bottom: 0.25rem;
    }
  
    .pb-xxl-2 {
      padding-bottom: 0.5rem;
    }
  
    .pb-xxl-3 {
      padding-bottom: 1rem;
    }
  
    .pb-xxl-4 {
      padding-bottom: 1.5rem;
    }
  
    .pb-xxl-5 {
      padding-bottom: 3rem;
    }
  
    .pb-xxl-6 {
      padding-bottom: 4rem;
    }
  
    .pb-xxl-7 {
      padding-bottom: 6rem;
    }
  
    .pl-xxl-0 {
      padding-left: 0rem;
    }
  
    .pl-xxl-1 {
      padding-left: 0.25rem;
    }
  
    .pl-xxl-2 {
      padding-left: 0.5rem;
    }
  
    .pl-xxl-3 {
      padding-left: 1rem;
    }
  
    .pl-xxl-4 {
      padding-left: 1.5rem;
    }
  
    .pl-xxl-5 {
      padding-left: 3rem;
    }
  
    .pl-xxl-6 {
      padding-left: 4rem;
    }
  
    .pl-xxl-7 {
      padding-left: 6rem;
    }
  
    .m-xxl-0 {
      margin: 0rem;
    }
  
    .m-xxl-1 {
      margin: 0.25rem;
    }
  
    .m-xxl-2 {
      margin: 0.5rem;
    }
  
    .m-xxl-3 {
      margin: 1rem;
    }
  
    .m-xxl-4 {
      margin: 1.5rem;
    }
  
    .m-xxl-5 {
      margin: 3rem;
    }
  
    .m-xxl-6 {
      margin: 4rem;
    }
  
    .m-xxl-7 {
      margin: 6rem;
    }
  
    .mt-xxl-0 {
      margin-top: 0rem;
    }
  
    .mt-xxl-1 {
      margin-top: 0.25rem;
    }
  
    .mt-xxl-2 {
      margin-top: 0.5rem;
    }
  
    .mt-xxl-3 {
      margin-top: 1rem;
    }
  
    .mt-xxl-4 {
      margin-top: 1.5rem;
    }
  
    .mt-xxl-5 {
      margin-top: 3rem;
    }
  
    .mt-xxl-6 {
      margin-top: 4rem;
    }
  
    .mt-xxl-7 {
      margin-top: 6rem;
    }
  
    .mr-xxl-0 {
      margin-right: 0rem;
    }
  
    .mr-xxl-1 {
      margin-right: 0.25rem;
    }
  
    .mr-xxl-2 {
      margin-right: 0.5rem;
    }
  
    .mr-xxl-3 {
      margin-right: 1rem;
    }
  
    .mr-xxl-4 {
      margin-right: 1.5rem;
    }
  
    .mr-xxl-5 {
      margin-right: 3rem;
    }
  
    .mr-xxl-6 {
      margin-right: 4rem;
    }
  
    .mr-xxl-7 {
      margin-right: 6rem;
    }
  
    .mb-xxl-0 {
      margin-bottom: 0rem;
    }
  
    .mb-xxl-1 {
      margin-bottom: 0.25rem;
    }
  
    .mb-xxl-2 {
      margin-bottom: 0.5rem;
    }
  
    .mb-xxl-3 {
      margin-bottom: 1rem;
    }
  
    .mb-xxl-4 {
      margin-bottom: 1.5rem;
    }
  
    .mb-xxl-5 {
      margin-bottom: 3rem;
    }
  
    .mb-xxl-6 {
      margin-bottom: 4rem;
    }
  
    .mb-xxl-7 {
      margin-bottom: 6rem;
    }
  
    .ml-xxl-0 {
      margin-left: 0rem;
    }
  
    .ml-xxl-1 {
      margin-left: 0.25rem;
    }
  
    .ml-xxl-2 {
      margin-left: 0.5rem;
    }
  
    .ml-xxl-3 {
      margin-left: 1rem;
    }
  
    .ml-xxl-4 {
      margin-left: 1.5rem;
    }
  
    .ml-xxl-5 {
      margin-left: 3rem;
    }
  
    .ml-xxl-6 {
      margin-left: 4rem;
    }
  
    .ml-xxl-7 {
      margin-left: 6rem;
    }
  }
  .p-0 {
    padding: 0rem;
  }
  
  .p-1 {
    padding: 0.25rem;
  }
  
  .p-2 {
    padding: 0.5rem;
  }
  
  .p-3 {
    padding: 1rem;
  }
  
  .p-4 {
    padding: 1.5rem;
  }
  
  .p-5 {
    padding: 3rem;
  }
  
  .p-6 {
    padding: 4rem;
  }
  
  .p-7 {
    padding: 6rem;
  }
  
  .pt-0 {
    padding-top: 0rem;
  }
  
  .pt-1 {
    padding-top: 0.25rem;
  }
  
  .pt-2 {
    padding-top: 0.5rem;
  }
  
  .pt-3 {
    padding-top: 1rem;
  }
  
  .pt-4 {
    padding-top: 1.5rem;
  }
  
  .pt-5 {
    padding-top: 3rem;
  }
  
  .pt-6 {
    padding-top: 4rem;
  }
  
  .pt-7 {
    padding-top: 6rem;
  }
  
  .pr-0 {
    padding-right: 0rem;
  }
  
  .pr-1 {
    padding-right: 0.25rem;
  }
  
  .pr-2 {
    padding-right: 0.5rem;
  }
  
  .pr-3 {
    padding-right: 1rem;
  }
  
  .pr-4 {
    padding-right: 1.5rem;
  }
  
  .pr-5 {
    padding-right: 3rem;
  }
  
  .pr-6 {
    padding-right: 4rem;
  }
  
  .pr-7 {
    padding-right: 6rem;
  }
  
  .pb-0 {
    padding-bottom: 0rem;
  }
  
  .pb-1 {
    padding-bottom: 0.25rem;
  }
  
  .pb-2 {
    padding-bottom: 0.5rem;
  }
  
  .pb-3 {
    padding-bottom: 1rem;
  }
  
  .pb-4 {
    padding-bottom: 1.5rem;
  }
  
  .pb-5 {
    padding-bottom: 3rem;
  }
  
  .pb-6 {
    padding-bottom: 4rem;
  }
  
  .pb-7 {
    padding-bottom: 6rem;
  }
  
  .pl-0 {
    padding-left: 0rem;
  }
  
  .pl-1 {
    padding-left: 0.25rem;
  }
  
  .pl-2 {
    padding-left: 0.5rem;
  }
  
  .pl-3 {
    padding-left: 1rem;
  }
  
  .pl-4 {
    padding-left: 1.5rem;
  }
  
  .pl-5 {
    padding-left: 3rem;
  }
  
  .pl-6 {
    padding-left: 4rem;
  }
  
  .pl-7 {
    padding-left: 6rem;
  }
  
  .m-0 {
    margin: 0rem;
  }
  
  .m-1 {
    margin: 0.25rem;
  }
  
  .m-2 {
    margin: 0.5rem;
  }
  
  .m-3 {
    margin: 1rem;
  }
  
  .m-4 {
    margin: 1.5rem;
  }
  
  .m-5 {
    margin: 3rem;
  }
  
  .m-6 {
    margin: 4rem;
  }
  
  .m-7 {
    margin: 6rem;
  }
  
  .mt-0 {
    margin-top: 0rem;
  }
  
  .mt-1 {
    margin-top: 0.25rem;
  }
  
  .mt-2 {
    margin-top: 0.5rem;
  }
  
  .mt-3 {
    margin-top: 1rem;
  }
  
  .mt-4 {
    margin-top: 1.5rem;
  }
  
  .mt-5 {
    margin-top: 3rem;
  }
  
  .mt-6 {
    margin-top: 4rem;
  }
  
  .mt-7 {
    margin-top: 6rem;
  }
  
  .mr-0 {
    margin-right: 0rem;
  }
  
  .mr-1 {
    margin-right: 0.25rem;
  }
  
  .mr-2 {
    margin-right: 0.5rem;
  }
  
  .mr-3 {
    margin-right: 1rem;
  }
  
  .mr-4 {
    margin-right: 1.5rem;
  }
  
  .mr-5 {
    margin-right: 3rem;
  }
  
  .mr-6 {
    margin-right: 4rem;
  }
  
  .mr-7 {
    margin-right: 6rem;
  }
  
  .mb-0 {
    margin-bottom: 0rem;
  }
  
  .mb-1 {
    margin-bottom: 0.25rem;
  }
  
  .mb-2 {
    margin-bottom: 0.5rem;
  }
  
  .mb-3 {
    margin-bottom: 1rem;
  }
  
  .mb-4 {
    margin-bottom: 1.5rem;
  }
  
  .mb-5 {
    margin-bottom: 3rem;
  }
  
  .mb-6 {
    margin-bottom: 4rem;
  }
  
  .mb-7 {
    margin-bottom: 6rem;
  }
  
  .ml-0 {
    margin-left: 0rem;
  }
  
  .ml-1 {
    margin-left: 0.25rem;
  }
  
  .ml-2 {
    margin-left: 0.5rem;
  }
  
  .ml-3 {
    margin-left: 1rem;
  }
  
  .ml-4 {
    margin-left: 1.5rem;
  }
  
  .ml-5 {
    margin-left: 3rem;
  }
  
  .ml-6 {
    margin-left: 4rem;
  }
  
  .ml-7 {
    margin-left: 6rem;
  }
  

```

