# Tree-sitter demo

Dette repo er et `minimum` proof-of-concept for om tree-sitter har god nok funksjonalitet for å transformere
repo [pensjons-regler](https://github.com/navikt/pensjon-regler), basert på [rule-dsl](https://github.com/navikt/rule-dsl), til en form for graf notasjon.

Hvis repo kan transformeres til en `god nok graf`, kan mye av samhandlingen mellom utviklere, funksjonelle og fag skje med graf.

Grafen kan kanskje tydeliggjøre behovet for omskriving av enkelte regler, hvorvidt `pakksedel` skal bli en `sti i grafen` mm.


## Minimum proof-of-concept

Begynner med pakken
`FastsettTrygdetidFlyt` - package no.nav.domain.pensjon.regler.repository.komponent.trygdetid.flyter

type `noder` å identifisere;
`AbstractRuleFlow` - som igjen er arvet til AbstractPensjonRuleflow, som igjen bruker arves til FastsettTrygdetidFlyt.

**Spørsmål** er det `godt nok` med `grandchildren` av AbstractRuleflow?

`forgreining`: -   
`gren`: -  
`betingelse{ uttrykk }`: -  
`flyt`:   
`regel (navn)`: -  
    `HVIS { uttrykk }`: -  
    `OG { uttrykk }`: -  
    `SÅ { statement }`: -    

Result: en enkel form for console output som viser relevant uttrekk.

## Bygg

Gjenbruk av samme maven versjon som `pensjon-regler`.



