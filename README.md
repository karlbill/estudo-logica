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
Sejam **p, q, r, s** proposições simples quaisquer.

#### Equivalências tautológicas
1. Indempotência (IND):
  >> **(p ^ p) $<->$ p <br>
  >> (p v p) $<->$ p**

2. Comutação (COM):
  >> **(p ^ q) $<->$ (q ^ p) <br>
  >> (p v q) $<->$ (q v p)**

3. Associação (ASS):
  >> **((p ^ q) ^ r) $<->$ (p ^ (q ^ r)) <br>
  >> ((p v q) v r) $<->$ (p v (q v r))** 

4. Distribuição (DIS):
  >> **(p ^ (q v r)) $<->$ ((p ^ q) v (p ^ r)) <br>
  >> (p v (q ^ r)) $<->$ ((p v q) v (p v r)) <br>
  >> (p $->$ (q ^ r)) $<->$ ((p $->$ q) ^ (p $->$ r)) <br>
  >> (p $->$ (q v r)) $<->$ ((p $->$ q) v (p $->$ r))**

5. Leis de Morgan (MOR):
  >> **~(p v q) $<->$ (~p ^ ~q) <br>
  >> ~(p ^ q) $<->$ (~p v ~q)**

6. Dupla Negação (D.N.):
  >> **~(~p) $<->$ p**

7. Equivalência Material (E.M.):
  >> **(p $<->$ q) $<->$ ((p $<->$ q) ^ (q $<->$ p)) <br>
  >> (p $<->$ q) $<->$ ((p ^ q) v (~p ^ ~q))**

8. Implicação Material (I.M.):
  >> **(p $->$ q) $<->$ (~p v q)** 

9. Negação da Implicação Material (N.I.M.):
  >> **~(p $->$ q) $<->$ (p ^ ~q)** 

10. Transposição (TRA):
  >> **(p $->$ q) $<->$ (~q $->$ ~p)** 

11. Importação / Exportação (I.E):
  >> **((p ^ q) $->$ r) $<->$ (p $->$ (q $->$ r))** 

12. Absurdo (ABD):
  >> **(p $->$ (q ^ ~q)) $<->$ ~p**

## Implicações Tautológicas
1. Adição (ADI)
  >> **p $->$ (p v q)** 

2. Simplificação (SIM)
  >> **(p ^ q) $->$ p**
  >> **(p ^ q) $->$ q**

3. Conjunção (CON)
  >> **(p ^ q) $->$ (p ^ q)**
  >> **(p ^ q) $->$ (q ^ p)**

4. Absorção (ABS)
  >> **(p $->$ q) $->$ (p $->$ (p ^ q))**

5. Modus Ponens (M.P.)
  >> **((p $->$ q) ^ p) $->$ q**

6. Modus Tollens (M.T.)
  >> **((p $->$ q) ^ ~q) $->$ ~p**

7. Dilema Construtivo (D.C.)
  >> **((p $->$ q) ^ (r $->$ s) ^ (p v r)) $->$ (q v s)**

8. Dilema Destrutivo (D.D.)
  >> **((p $->$ q) ^ (r $->$ s) ^ (~q v ~s)) $->$ (~p v ~r)**

9. Silogismo Disjuntivo (S.D.)
  >> **((p v q) ^ ~p) $->$ q **
  >> **((p v q) ^ ~q) $->$ p **

10. Silogismo Hipotético (S.H.)
  >> **((p $->$ q) ^ (q $->$ r)) $->$ (p $->$ r)**

11. Exportação (EXP)
  >> **((p ^ q) $->$ r) $->$ (p $->$ (q $->$ r))**

12. Importação (IMP)
  >> **(p $->$ (q $->$ r)) $->$ ((p ^ q) $->$ r)**

## Outras tautologias
1. Princípio da Identidade
  >> **p $->$ p**

2. Princípio da Não-contradição
  >> **~(p ^ ~p)**

3. Princípio do Terceiro Excluído
  >> **p v ~p**

## Regras de dedução do cálculo proposicional
1. Introduzir premissas através de: Equivalências Tautológicas, Implicações Tautológicas e do Teorema da Dedução;
2. Indicar ao lado de cada nova premissa a tautologia e o número das linhas englobadas na tautologia;
3. Refazer os procedimentos até a conclusão.
> Sendo a conclusão, após a aplicação dos procedimentos acima, a mesma conclusão inicial, então a prova de validade estará finalizada.
> 
> Obs: é importante lembrar que em uma Implicação Tautológica, a recíproca não é verdadeira, apenas na Equivalência Tautológica. Ou seja, a partir de uma conclusão, não podemos deduzir as premissas, no caso da Implicação Tautológica.

> Exemplo: Ou votamos no candidato A ou festejaremos na rua. Decidimos não votar no candidato A. Logo, festejaremos na rua.
> V: votar no candidato A
> F: festejar na rua
> 1. V v F
> 2. ~V
> 3. Portanto, F
> 
> Equivale a: **(V v F) ^ ~V $->$ F**
> 
> 4. F  (Uso do **Silogismo Disjuntivo** nas premissas 1 e 2).


## Teorema da Dedução
Estabelecido por Jacques Herbrand (1930) e por Alfred Tarski (1936).

Observemos a equivalência tautológica (**Importação/Exportação**) dos argumentos:
> 1. **A$_1$ ^ A$_2$ ^ A$_3$ ^ A$_(n-1)$ $->$ (B $->$ C)**
> 2. **A$_1$ ^ A$_2$ ^ A$_3$ ^ A$_(n-1)$ ^ B $->$ C**
>
> Se provarmos a equivalência tautológica de 2, então a validade de 1 também estará provada.
>
> Se **Γ = {A1, A2, ..., An–1}** é o conjunto de premissas de um argumento, **B** é introduzida como premissa e **C** é consequência de **Γ** e **B**, 
> 
> então **B → C** será consequência de **Γ**, 
> 
> ou ainda:
> 
> **Se Γ, B ⊢ C, então Γ ⊢ B → C**

### Prova Indireta da Validade 
Introdução de uma nova premissa que negue a conclusão e, a partir dela, apresente uma contradição. Dessa contradição é extraída a validade do argumento.

### Prova Indireta de Invalidade (Redução ao Absurdo)
Se a partir de uma hipótese **¬φ** derivarmos uma contradição,então podemos admitir **φ**.

## Prova de Invalidade
Será apresentada uma forma de prova sem o uso da Tabela-Verdade que, dependendo da quantidade de premissas, se torna inviável.
> Parte-se da ideia de que, para invalidar um argumento, todas as suas premissas devem ser Verdadeiras, enquanto a sua conclusão for Falsa.
> 
> Se **V $->$ F** é a única forma dessa condicional ser Falsa.

### Método da Atribuição de Valores
1. Atribui-se o valor **F** para a Conclusão
2. Atribui-se valor-verdade **V** para as demais premissas.




## Referência Bibliográfica:
BISPO, Carlos A., CASTANHEIRA, Luiz B., FILHO, Oswvaldo M.S., Introdução à Lógica Matemática, Cengage Learning, 2012.
