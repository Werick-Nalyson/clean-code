# clean-code
Código limpo é um código fácil de ser entendido.

### 1. Variáveis:
- Deixar as variáveis sempre o mais descritivas possíveis e de acordo com a responsabilidade dela.
- Não abreviar variáveis (Ex.: let couter para let c).
- Evitar redundâncias.

### 2. Funções:
- Cada função deve ter apenas uma responsabilidade
- Sempre começar com um verbo. (ex.: getUserData)

### 3. Comentários:
- Na maioria das vezes mais atrapalha do que ajuda
- Podem ficar desatualizados
- Podem ser redundantes

#### 3.1 Comentários úteis:
- Para descrever algum bug
- Para descrever uma regra de negócio

### 4. Números mágicos:
- Sempre delcarar números.

Ex.: const AN_HOUR_IN_MILISECOUND = 3600000
     setTimeout(console.log("Hello World"), AN_HOUR_IN_MILISECOUND)

### 5. Anti pattern (Anti padrão):
- Um padrão ruim de código

Ex.: (React):
- Prop Drilling: É quando uma propriedade caminha para níveis muito abaixo na aplicação, passando de componente por componente.
  Resolução: utilizar uma única fonte de dados, ex.: Redux, ContexAPI

- Mal uso das keys
  Resolução: A key deve ser única e previsível

- Componentes que retornam muitos outros diferentes
  Resolução: Criar mini componentes (Ao invés de criar como um componente global, criar um que apenas aquela ṕágina vai retornar)

### 6. Code smell (Código com pouca legibilidade e quase se encaixando em um Anti pattern)
- Múltiplos níveis de identação
  Resolução: Early return ou cláusula de guarda

- Funções que recebem muitos parâmetros / Funções muito longas
  Resolução: Dividir essa função em outras menores

### ALGUNS CONCEITOS IMPORTANTES

- DRY (Don't repeat yourself - Não se repita): É quando há existência de um código, regra de negócio que é usado por muitas funções porém este código está sendo repetio em cada uma delas. Sendo assim, quando uma for alterada a outra também precisará ser. Se esse determinado bloco de código ficasse limitado em uma função especifica, o problema seria solucionado.

- KISS (Keep it simple stupid - Mantenha simples): Deixar o código o mais simples possível, para que outros devs entendam.

- YAGNI (You ain't gonna need it - Você não vai precisar disso): Não é só porque algo novo lançou ou todos estão usando, que você também deva. Primeiro deve-se analisar sua situação e ver se aquilo é necessário.

Sempre usar linters - padronização de código e boas práticas.
