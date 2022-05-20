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

