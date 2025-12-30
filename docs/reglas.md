Reglas del sistema de turnos:
- Un turno tiene fecha, hora, cliente y estado
- Estados posibles: pendiente, cancelado, atendido
- No se permiten turnos duplicados

- Un turno representa:

“Una reserva de atención en una fecha y hora para una persona, con un estado”.

Eso implica estado y tiempo.
No es solo “un objeto”.

- 3️⃣ Datos mínimos (decisión consciente)

Un turno DEBE tener:

id

Único

No depende de la posición en el array

No se reutiliza

fecha

Día del turno

No fecha completa con hora (separar conceptos)

hora

Hora específica del turno

cliente

Nombre o identificador simple

estado

Situación actual del turno

- ❌ Datos que NO vas a poner (a propósito)

Teléfono

Email

Duración

Observaciones

Precio

👉 Esto es lógica, no un sistema comercial completo.

- 4️⃣ Estados posibles (decisión CLAVE)

Definí explícitamente los estados válidos.

Solo estos tres:

pendiente

cancelado

atendido

- ⚠️ Regla importante:

Un turno NUNCA se elimina, solo cambia de estado.

Esto es pensamiento de sistemas y lo vas a ver mil veces en EDA y backend.

- Ejemplo conceptual (NO código):

Primer turno → id 1

Segundo → id 2

Tercero → id 3