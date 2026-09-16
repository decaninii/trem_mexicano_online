# Changelog

## v4
- Corrigido: trem só abre quando o dono realmente não consegue jogar (jogar em outro lugar por escolha não abre mais)
- Corrigido: duplo trava a mesa até ser coberto (mesmo jogador tenta primeiro, depois passa a vez para o próximo)
- Corrigido: Trem Mexicano fica fechado só na primeira jogada de cada rodada, liberando a partir da segunda em diante
- Peças, cadeado/bolinha e rótulos maiores no tabuleiro, para melhor legibilidade
- Alertas: duplo aberto (banner fixo) e jogador com 1 peça na mão (destaque piscando na lista de jogadores)
- Ajuste de layout mobile: painel "você pode jogar em" compacto, tabuleiro sempre com espaço garantido na tela

## v3
- Zoom e pan persistentes no tabuleiro, com suporte a pinça (dois dedos) no celular
- Modo "jogar contra o computador" (2 a 8 jogadores, 3 níveis de dificuldade)
- Arrastar peça na mão para reordenar (além dos botões ◀ ▶)
- Cor diferente por número (0–12) nas peças, para leitura mais rápida

## v2
- Cor por jogador, escolhida na sala de espera
- Reordenar peças da mão (botões)
- Contador de peças já jogadas por número (de 13 possíveis)
- Tabuleiro radial visual (peças saindo do centro, como o jogo físico) substituindo a lista em texto
- Corrigida a orientação de exibição das peças no trem (a extremidade de conexão sempre aparece primeiro)

## v1
- MVP inicial: motor de regras completo (duplo-12, até 8 jogadores, trens, duplo, pontuação em 13 rodadas)
- Salas por código, sincronização via armazenamento de artifact do Claude
