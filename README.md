# MIDuIno

Controlador MIDI baseado no código de https://github.com/NotesAndVolts

Alterações feitas:

Configurado para 4 pots, 1 mux e 8 muxpots.

Entrada A0 está reservada para pitch bend, já que bend não é um CC. Função updatePots() alterada de acordo (pitch bend acionado via eixo Y de joystick analógico).

Entrada A4 está reservada para seletor de canais (1 a 12, não configurado como pot). Funções updatePots() e updateMuxPots() alteradas de acordo (analogRead(A4) definindo canal em vez de código fixo), funções restantes ignoradas.

Entrada digital 13 reservada para botão que alterna valor invertido para sliders (POTS[>2] e MUXPOTS). setup(), loop(), updatePots() e updateMuxPots() alterados de acordo. Bool "_invertido" declarado.

A fazer:

Testar inversão dos sliders.

