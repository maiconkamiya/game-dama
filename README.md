Foi utilizado CDN VueJS

```
<script src="https://unpkg.com/vue@2"></script>
```

# Desafio técnico
##### Foco Front-end

## Objetivo e linha de avaliação

Este desafio tem como objetivo verificar habilidades e familiaridade com desenvolvimento front-end em nível pleno ou superior.
Avalia-se a capacidade de montar elementos na página por meio de CSS, bem como a capacidade de aplicar estilo de forma programática (não estática) à um elemento de acordo com interações do usuário.
Verifica-se também a capacidade de seguir uma guia/determinação visual especificada com algum nível de detalhe, porém mantendo a expectativa de interpretação do candidato.

## Tema

Damas é um jogo popular de tabuleiro 8 x 8 em que as peças ocupam somente as casas de uma determinada cor. As peças movem-se somente na diagonal e para casas desocupadas.
Nesse desafio busca-se implementar um subconjunto desses movimentos, **não sendo necessário implementar todo o jogo**.

## Recursos a serem implementados:
### Estrutura básica da página

A interface está dividida em três blocos:
- Uma coluna com 2 / 3 da página contendo o tabuleiro em si
- Outra coluna, com dois blocos dispostos na vertical para configurações
    - O bloco superior contém uma opção para mudar a cor das peças dos jogadores
- A altura atribuida às duas caixas da segunda coluna deve ser a mesma da caixa atribuida ao jogo.

### Estado inicial
- Na inicialização da aplicação, todas as peças devem ocupar as casas iniciais de cor escura mais próximas do seu jogar, nas duas primeiras fileiras
- Cada jogador tem uma cor atribuída às suas peças
    - Jogador Alfa: peças pretas
    - Jogador Beta: peças vermelhas
- A interface está dividida em três blocos:
    - Uma coluna com 2 / 3 da página contendo o tabuleiro em si
    - Outra coluna, com dois blocos dispostos na vertical para configurações
        - O bloco superior contém uma opção para mudar a cor das peças dos jogadores. Ao utilizar essa opção, a cor das peças deve mudar instantaneamente no tabuleiro, sem refresh
        - O bloco inferior contém uma opção para reiniciar o jogo. Ao acionar essa opção a aplicação deve voltar ao estado inicial sem dar refresh na página. Essa opção não deve resetar as cores das peças.

### Movimentos válidos
- Uma peça só pode se mover na diagonal e para uma casa de fileira adjacente (tanto para frente como para trás)
- Uma peça só pode se mover para uma casa desocupada
- Não é necessário implementar turno (vez) do jogador. Pode ser possível mover qualquer peça a qualquer momento, desde que seguindo os critérios anteriores
- Se o jogador tentar mover a peça para uma casa inválida, desconsidere sua ação
- **Interação visual:**
    - Deseja-se usar drag-and-drop (arrastar) para mover a peça de uma casa para outra.
- Frise-se: não é esperado implementar o jogo. Somente alguns dos movimentos e validações para a finalidade dessa avaliação.

### Considerações tecnológicas e estéticas
- Espera-se o emprego de VueJs ou ReactJs para a implementação dos componentes visuais
- Deve haver um componente específico representando a peça.
- Você pode usar a forma que achar mais adequada para controlar o estado do jogo, cores das peças e ações mencionadas.
- As peças e tabuleiro devem obrigatoriamente ser construídos usando elementos HTML e não imagens ou gráficos pré-criados.
- Animações são desnecessárias
- Alinhe os elementos de forma harmônica (peça dentro da casa, distâncias entre elementos e bordas, etc)

### Entrega
- Deve ser entregue um único repositório git com tudo o que for necessário para executar a aplicação localmente em ambiente de teste
- A aplicação não deve depender de pacotes instalados no sistema para além do NPM ou YARN como gestão de dependências
- Informe no README.md do projeto quaisquer dependências externas utilizadas e a sua motivação.
- A aplicação deve ser capaz de iniciar utilizando os comandos abaixo (ou a versão equivalente com yarn)

```
npm install
npm start
```
