# Estudo de Lógica: Cálculo de Predicados
#### O estudo agora passa à análise da **estrutura de uma proposição simples**: um **sujeito** e um **predicado**.

## Termo e Predicado
> 1. Termo: o Sujeito da sentença declarativa. (letra minúscula)
> 2. Predicado: o que se declara a respeito do termo. (letra maiúscula)
>
> Exemplo: Pedro é médico.
>
> Termo: Pedro
> Predicado: é médico.
> 
> Representação: $M_p$

## Função Proposicional
Nas funções proposicionais os **termos são variáveis(x)**, onde **Ω** representa o **conjunto de todos os termos**.

## Quantificadores
Operadores lógicos que restringem as funções proposicionais, de forma que elas se refiram a todo o conjunto ou a uma parte dele. Há dois quantificadores:
1. **∀** (quantificador universal): para todo, qualquer que seja etc.
2. **∃** (quantificador existencial): existe, há, alguns etc.

### Formalização do cálculo de predicados
Em **funções proposicionais quantificadas universalmente**:
> Exemplo: Todo **A** tem a propriedade **B**.
>
> usa-se a letra **x** como representante de qualquer *termo* do **conjunto Ω**, expressando:
>
> **Qualquer que seja x, se x tem a propriedade a A, então x tem a propriedade B**.
>
> Simbolicamente:
>
> **∀x (Ax → Bx)**

Em **funções proposicionais quantificadas existencialmente**:
> Exemplo: Existe pelo menos um x que tem a propriedade a A e a propriedade **B**.
>
> **Existe pelo menos um x que tem a propriedade a A e a propriedade B**.
>
> Simbolicamente:
>
> **∃x (Ax ∧ Bx)**

## Regras de formação do cálculo de predicados
1. Um *predicado* **P** seguido de um *termo* **x** é uma *wff* simbolizada por $P_x$
2. $P_x$ é *wff* $->$ ~$P_x$ é *wff*
3. $P_x$ e $Q_x$ são *wff* $->$ $P_x$ ^ $Q_x$ , $P_x$ v $Q_x$ , $P_x$ $->$ $Q_x$ , $P_x$ $<->$ $Q_x$ são *wff*
4. $P_x$ $->$ é *wff* $->$ ∀x (Px) e ∃x (Px) também são *wff*

## Equivalência entre quantificadores
Útil para transformarmos as funções proposicionais quatificadas em sua forma não negativa, o que facilita a prova de sua validade.

- Equivalências:
1. **¬∃x (αx)** é equivalente a **∀x ¬(αx)**   Não existe um *termo* **x** associado ao *predicado* **α** $<=>$ todo *termo* **x** não está associado ao *predicado* **α**
2. **¬∀x (αx) é equivalente a ∃x ¬(αx)**    Não é todo **x** que está associado ao *predicado* **α** $<=>$ existe pelo menos um **x** que não está associado a **α**
> Exemplo: Nem todos os animais não são domésticos.
>
> ¬∀x ¬(Ax ∧ Dx)    Tradução simbólica
>
> ∃x ¬¬(Ax ∧ Dx)    Equivalência 2
>
> ∃x (Ax ∧ Dx)      Dupla Negação
>
> Tradução para linguagem natural:
> Existe animal doméstico. 
> Alguns animais são domésticos.

# Capítulo 7: Validade de Argumentos com Quantificadores
Provar a validade de argumentos que envolvam funções proposicionais quantificadas, transformando tais argumentos por meio da *exemplificação*, sem quantificadores. Terminada a prova de validade do argumento exemplificado, usa-se a *generalização* para obter a conclusão do argumento quantificado.

- Exemplificação: aplicação de duas tautologias que efetuam a passagem de funções proposicionais para proposições.
- Generalização: reverte o que a exemplificação realiza, tranformando proposições em funções proposicionais.

## Exemplificação Existencial (E.E.)
**∃x (αx) $->$ αc** 
> Se existe um termo x associado ao predicado α, estipulamos que este termo seja c.

## Exemplificação Universal (E.U.)
**∀x (αx) $->$ αc**
> Se todos os termos estão associados ao predicado α, escolhemos um deles, c, um termo constante.

## Generalização Existencial (G.E.)
**αc $->$ ∃x (αx)** 
> Se concluirmos que um termo c está associado ao predicado α, então existe ao menos um termo associado a α.

## Generalização Universal (E.U.)
**αc $->$ ∀x (αx)**
> Se o termo c tomado na exemplificação pode ser qualquer um, então qualquer termo está associado a α.

**Obs: a Exemplificação Existencial sempre deve ser executada antes da Exemplificação Universal.**


## Referência Bibliográfica:
BISPO, Carlos A., CASTANHEIRA, Luiz B., FILHO, Oswvaldo M.S., Introdução à Lógica Matemática, Cengage Learning, 2012.
