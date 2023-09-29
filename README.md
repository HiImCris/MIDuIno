# MIDuIno

Controlador MIDI baseado no código de https://github.com/NotesAndVolts

Alterações feitas:

Configurado para 4 pots, 1 mux e 8 muxpots.

Entrada A0 está reservada para pitch bend, já que bend não é um CC. Função updatePots() alterada de acordo (pitch bend acionado via eixo Y de joystick analógico).

Entrada A4 está reservada para seletor de canais (0 a 11, não configurado como pot). Funções updatePots() e updateMuxPots() alteradas de acordo (analogRead(A4) definindo canal em vez de código fixo), funções restantes ignoradas.


A fazer:

Implementar inversão da leitura dos potenciômetros a partir de click no joystick (push button).

      ↳Excluir pots A1 e A2 (além do bend), pois a ideia é implementar essa função só para meus sliders.

