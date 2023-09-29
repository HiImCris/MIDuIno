# MIDUino

Controlador MIDI baseado no código de https://github.com/NotesAndVolts

Alterações feitas:
Entrada A0 está reservada para pitch bend. Função updatePots() alterada de acordo.
Entrada A4 está reservada para seletor de canais (0 a 11) Funções updatePots() e updateMuxPots() alteradas de acordo (analogRead(A4) definindo canal em vez de código fixo), funções restantes ignoradas.
.

