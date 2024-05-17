# MIDuIno

Controlador MIDI baseado no código de https://github.com/NotesAndVolts

Alterações feitas:
Configurado para 3 pots, 1 mux e 8 muxpots.
Entrada A5 está reservada para seletor de canais (1 a 12). Funções updatePots() e updateMuxPots() alteradas de acordo (analogRead(A5) definindo canal em vez de código fixo), funções restantes ignoradas.

Hardware:
9 sliders, 2 knobs, 1 chave seletora, um botão chave seletora

Chave seletora: contatos ligados via resistores, funciona como potenciômetro de posições fixas. Serve para configurar canal.
Botão chave seletora: switch de duas posições, recebe um par de inputs e conecta a um de dois pares de output. Deveria servir como inversor de sliders.

Problemas:
Leituras aleatórias, principalmente quando o botão é pressionado. Dificulta até mesmo o monitoramento dos valores.

Leituras inconsistentes.

Botão não inverte a leitura dos sliders, mas aparentemente transforma a curva numa parábola. O motivo disso é porque eu sou burro e ainda não entendi como potenciômetros funcionam. (Ou meu multímetro só serve para medir potenciômetro no Mundo das Ideias, não aqueles que serão usados em circuitos.)

Leitura do seletor de canais inconsistente. Talvez programar valores diferentes resolva o problema.


Protótipo:
![alt text](https://github.com/HiImCris/MIDuIno/blob/main/Prototipo.jpg?raw=true)

