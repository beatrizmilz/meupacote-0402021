
<!-- README.md is generated from README.Rmd. Please edit that file -->

# meupacote

<!-- badges: start -->

[![R-CMD-check](https://github.com/clente/meupacote/workflows/R-CMD-check/badge.svg)](https://github.com/clente/meupacote/actions)
<!-- badges: end -->

O objetivo do pacote é disponibilizar funções para analisar dados do
Brasileirão.

## Installation

And the development version from [GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("beatrizmilz/meupacote")
```

## Exemplo de uso

``` r
library(meupacote)
```

Nomes dos times que estão na base de dados:

``` r
unique(partidas_brasileirao$quem_ganhou)
#>  [1] "Athletico PR"  "Guarani"       "Atlético MG"   "Empate"       
#>  [5] "Criciúma"      "Grêmio"        "Internacional" "Flamengo"     
#>  [9] "Vasco"         "Cruzeiro"      "Vitória"       "Ponte Preta"  
#> [13] "Paraná"        "São Caetano"   "Paysandu"      "Corinthians"  
#> [17] "Santos"        "Juventude"     "Bahia"         "Fluminense"   
#> [21] "São Paulo"     "Fortaleza"     "Coritiba"      "Goiás"        
#> [25] "Figueirense"   "Palmeiras"     "Botafogo"      "Brasiliense"  
#> [29] "Santa Cruz"    "Sport"         "América RN"    "Náutico"      
#> [33] "Ipatinga"      "Portuguesa"    "Santo André"   "Barueri"      
#> [37] "Avaí"          "Ceará"         "Atlético GO"   "América MG"   
#> [41] "Chapecoense"   "Joinville"     "CSA"           "Bragantino"
```

Como usar a função:

``` r
encontrar_pior_ano_time(time = "Corinthians") %>%
  knitr::kable()
```

| temporada | time        | n\_vitorias |
|----------:|:------------|------------:|
|      2007 | Corinthians |          10 |
