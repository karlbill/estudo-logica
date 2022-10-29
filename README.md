# Estudo de Lógica: Consequência Lógica ou Dedução Formal
#### Estudo da Consequência Lógica

## Introdução
**Consequência lógica** está na raiz da ideia de **raciocínio** (encadeamento de pensamentos). Porém, no contexto da Lógica, chamamos a essas atividades mentais de pensamentos ordenados de *argumento*.
> **Argumento**: **conjunto de n proposições**, ou de fórmulas, nas quais *uma delas (a conclusão) é consequência das outras (premissas)*. 
>
> A essa derivação (consequência) chamamos de *dedução*, de **natureza puramente formal na Lógica Matemática**.

O conceito de *consequência lógica* pode ser associado não só à noção de *prova matemática* como também à aplicação de *regras de inferência*. Da mesma forma, podemos associá-la às noções de *computabilidade* e de *algoritmo*.

Diposição de um argumento:
> $P_1$  <br>
> $P_2$  <br>
> ... <br>
> $P_(n-1)$ <br>
> Portanto, **C.**   ( $P_n$ = C )

Equivalente a: $P_1$ ^ $P_2$ ^ ... ^ $P_(n-1)$ $->$ C.

Passos para a transformação simbólica:
> 1. Cada premissa em uma linha numerada, seguindo a ordem crescente dos números naturais;
> 2. A Conclusão é a última proposição;
> 3. Cada proposição simples componente das premissas é representada por uma letra maiúscula ligada à sua palavra-chave.

Palavras indicadoras de Premissas e Conclusão: 
>| Premissas          | Conclusão          |
>|     :---:          |      :---:         |
>| pois               | portanto           |
>| desde que          | logo               |
>| como               | dessa maneira      |
>| porque             | consequentemente   |
>| assumindo que      | assim sendo        |
>| visto que          | segue que          |
>| admitindo que      | de modo que        |
>| dado que           | resulta que        |
>| supondo que        | então              


##Validade de um argumento
Um argumento é válido se, e somente se, for uma implicação tautológica, sendo impossível todas as *premissas* serem Verdadeiras e a *conclusão* ser Falsa.

> Exemplo: Dado um argumento qualquer
>
> $P_1$  <br>
> $P_2$  <br>
> ... <br>
> $P_(n-1)$ <br>
> Portanto, **C.** <br>
>
> Equivalente a: $P_1$ ^ $P_2$ ^ ... ^ $P_(n-1)$ $->$ C.
>
> Se a conclusão C puder ser deduzida das premissas $P_1$, $P_2$, ..., $P_(n-1)$, então o argumento é válido e pode ser escrito assim:
>
> $P_1$, $P_2$, ..., $P_(n-1)$ $|-$ C , onde $|-$ é chamado *traço de asserção* (afirma que a proposição à direita pode ser deduzida das premissas à esquerda).

**Um *argumento é inválido* somente quando *todas as suas premissas são verdadeiras* e a *conclusão é falsa*.**

### (In)Validade x Valor-verdade
A *Verdade* e a *Falsidade* são *propriedades das proposições*, enquanto a *Validade* e a *Invalidade* são *propriedades dos argumentos*. O **Valor-verdade** depende do *contexto*, enquanto a *Validade* depende da *forma*.

## Prova direta de validade
Outra maneira de se provar a validade de um argumento, utilizando: *implicações* e *equivalências tautológicas*.

### Tautologias úteis ###
Sejam p, q, r, s proposições simples quaisquer.

#### Equivalências tautológicas
1. Indempotência (IND):
  >> (p ^ p) $<->$ p <br>
  >> (p v p) $<->$ p

2. Comutação (COM):
  >> (p ^ q) $<->$ (q ^ p) <br>
  >> (p v q) $<->$ (q v p)

3. Associação (ASS):
  >> ((p ^ q) ^ r) $<->$ (p ^ (q ^ r)) <br>
  >> ((p v q) v r) $<->$ (p v (q v r)) 

4. Distribuição (DIS):
  >> (p ^ (q v r)) $<->$ ((p ^ q) v (p ^ r)) <br>
  >> (p v (q ^ r)) $<->$ ((p v q) v (p v r)) <br>
  >> (p $->$ (q ^ r)) $<->$ ((p $->$ q) ^ (p $->$ r)) <br>
  >> (p $->$ (q v r)) $<->$ ((p $->$ q) v (p $->$ r))

5. Leis de Morgan (MOR):
  >> ~(p v q) $<->$ (~p ^ ~q) <br>
  >> ~(p ^ q) $<->$ (~p v ~q)

6. Dupla Negação (D.N.):
  >> ~(~p) $<->$ p

7. Equivalência Material (E.M.):
  >> (p $<->$ q) $<->$ ((p $<->$ q) ^ (q $<->$ p)) <br>
  >> (p $<->$ q) $<->$ ((p ^ q) v (~p ^ ~q))

8. Implicação Material (I.M.):
  >> (p $->$ q) $<->$ (~p v q) 

9. Negação da Implicação Material (N.I.M.):
  >> ~(p $->$ q) $<->$ (p ^ ~q) 

10. Transposição (TRA):
  >> (p $->$ q) $<->$ (~q $<->$ ~p) 

11. Importação / Exportação (I.E):
  >> ((p ^ q) $->$ r) $<->$ (p $->$ (q $->$ r)) 

12. Absurdo (ABD):
  >> (p $->$ (q ^ ~q)) $<->$ ~p


## Referência Bibliográfica:
BISPO, Carlos A., CASTANHEIRA, Luiz B., FILHO, Oswvaldo M.S., Introdução à Lógica Matemática, Cengage Learning, 2012.
