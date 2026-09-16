# Trem Mexicano — Dominó Online

MVP de um jogo multiplayer de Trem Mexicano (dominó), com tabuleiro visual, regras clássicas implementadas e modo contra o computador.

## Estado atual

Este é um **protótipo funcional**, construído e testado inteiramente dentro do Claude (via artifacts). Ele **só funciona de verdade dentro do Claude.ai**: a sincronização entre jogadores depende de uma API de armazenamento (`window.storage`) que só existe no ambiente de artifacts do Claude. Se este arquivo for hospedado sozinho (Vercel, GitHub Pages etc.), a interface carrega, mas o multiplayer não sincroniza.

Ou seja: por enquanto este repositório é o **histórico de versões e ponto de partida** para uma futura reescrita com backend próprio — ainda não é o app final para publicar.

## Funcionalidades já implementadas

- Duplo-12 completo (91 peças), 2 a 8 jogadores
- Salas por código, com reconexão automática
- Trens individuais, Trem Mexicano, regra de duplo (trava a mesa até ser coberto), trem que só abre quando o dono realmente não consegue jogar
- Trem Mexicano fechado até o fim da primeira jogada de cada rodada
- Pontuação em 13 rodadas (duplo-12 até duplo-0), ranking final
- Tabuleiro radial (peças saindo do centro, como o jogo físico), com zoom e pan — inclusive pinça no celular
- Cor por jogador, indicador de trem aberto/fechado, alerta de duplo aberto e de "1 peça na mão"
- Contador de peças já jogadas por número
- Modo contra o computador (2 a 8 jogadores, 3 níveis de dificuldade)
- Reordenar peças da mão (arrastando ou com botões)

## Próximos passos (visão de produto)

Para virar um jogo publicável e monetizável, falta: backend com autoridade sobre as jogadas (anti-cheat), conexão em tempo real (WebSocket), banco de dados, autenticação via provedor gerenciado (Clerk/Auth0/Supabase Auth), pagamentos (Stripe/Mercado Pago) e adequação à LGPD.

## Como testar agora

1. Abra `trem-mexicano.html` como um artifact no Claude.
2. Publique o artifact e compartilhe o link com quem for jogar.
3. Um jogador cria a sala (recebe um código de 4 letras); os outros entram com o mesmo código.
