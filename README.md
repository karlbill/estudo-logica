# Estudo de Lógica: Tabela-verdade
#### Instrumento para determinação de todas as possíveis combinações dos valores-verdade das proposições simples.

## Introdução
O valor-verdade de uma proposição composta é obtido de forma única a partir dos valores-verdade atribuídos às proposições simples que a compõem.
> Obs: a atribuição de um valor-verdade para uma proposição simples depende de seu contexto e faz parte do estudo semântico.

Tabela-Verdade de Proposições Simples (quaisquer): **p** e **q**:
>|      |      |      |      |  Conj. | Disj. | Cond.  | Bicond. |
>| :--: | :--: | :--: | :--: |  :--:  |  :--: |  :--:  |   :--:  |
>|  p   |   q  |  ~p  |  ~q  |  p ^ q | p v q | p -> q | p <-> q |
>|  V   |   V  |   V  |  V   |   V    |   V   |   V    |    V    |
>|  V   |   F  |   V  |  F   |   F    |   V   |   F    |    F    |
>|  F   |   V  |   F  |  V   |   F    |   V   |   V    |    F    |
>|  F   |   F  |   F  |  F   |   F    |   F   |   V    |    V    |
 
O número de linhas de uma Tabela-Verdade depende do número de proposições simples presentes. 
> Fórmula: $2^n$, sendo n o número de proposições simples.


# Capítulo 3: Classificação das Proposições
#### As proposições compostas podem ser de 3 tipos: Tautológicas, Contraditórias e Contingentes.

- **Proposição Composta Tautológica**: são sempre Verdadeiras, independente do valor lógico atribuído a cada uma de suas premissas simples.
- **Proposição Composta Contraditória**: são sempre Falsas, independente do valor lógico atribuído a cada uma de suas premissas simples.
- **Proposição Composta Contingente**: podem ser Falsas ou Verdadeiras, dependendo do valor lógico atribuído às suas sentenças simples.

# Capítulo 4: Tautologias

- **Implicação tautológica**: é uma proposição condicional tautológica. 
> Exemplo: p ^ q -> p
>|  p   |   q  |  p ^ q | **p ^ q -> p** |
>| :--: | :--: |  :--:  |       :--:     |
>|  V   |   V  |   V    |      **V**     |
>|  V   |   F  |   F    |      **V**     |
>|  F   |   V  |   F    |      **V**     |
>|  F   |   F  |   F    |      **V**     |
>
> Ou seja: **p ^ q implica tautologicamente p**.

**Obs: A implicação tautológica é fundamental para o estudo da validade de um argumento.**

- **Equivalência Tautológica**: quando uma proposição bicondicional é tautológica.
> Exemplo: **~(p ^ q) <-> (~p v ~q)**
> (Equivalência tautológica denominada **Lei de Morgan**.)
>|  p   |   q  |  ~p  |  ~q  |  p ^ q | ~(p ^ q) | ~p v ~q | ~(p^q) <-> (~p v ~q) |
>| :--: | :--: | :--: | :--: |  :--:  |   :--:   |   :--:  |           :--:       |
>|  V   |   V  |   V  |  V   |   V    |     F    |    F    |            V         |
>|  V   |   F  |   V  |  F   |   F    |     V    |    V    |            V         |
>|  F   |   V  |   F  |  V   |   F    |     V    |    V    |            V         |
>|  F   |   F  |   F  |  F   |   F    |     V    |    V    |            V         |

Propriedades:
1. Reflexiva
  - **p -> p**                                (implicação tautológica)
  - **p <-> p**                               (equivalência tautológica)
2. Simétrica
  - **(p <-> q) |-- (q -> p)**                (implicação tautológica)
3. Transitiva
  - **(p -> q) ^ (q ^ r) -> (p -> r)**        (implicação tautológica)
  - **(p <-> q) ^ (q <-> r) |-- (p <-> r)**   (implicação tautológica) 


## Referência Bibliográfica:
BISPO, Carlos A., CASTANHEIRA, Luiz B., FILHO, Oswvaldo M.S., Introdução à Lógica Matemática, Cengage Learning, 2012.








