# MIDuIno

Controlador MIDI baseado no código de https://github.com/NotesAndVolts

Alterações feitas:

Entrada A0 está reservada para pitch bend. Função updatePots() alterada de acordo (pitch bend acionado via eixo Y de joystick analógico).

Entrada A4 está reservada para seletor de canais (0 a 11). Funções updatePots() e updateMuxPots() alteradas de acordo (analogRead(A4) definindo canal em vez de código fixo), funções restantes ignoradas.


A fazer:

Implementar inversão da leitura dos potenciômetros a partir de click no joystick (push button). [Decidir se inversão afetara só sliders ou todos os pots.]

