# 📄 Requerimiento Funcional
## Pago con código QR vía PIX – Mercado Pago (Brasil)

---

### 🎯 Objetivo
Permitir que un usuario realice un pago escaneando un código QR mediante el método PIX, visualizando previamente el monto y los datos del comercio, y confirmando el pago de forma segura.

---

### 👤 Actor principal
Usuario de la aplicación Mercado Pago.

---

### 📌 Precondiciones
- El usuario tiene sesión iniciada en la aplicación.
- El usuario cuenta con saldo disponible en su cuenta.
- El comercio genera un código QR válido.
- El dispositivo tiene cámara habilitada.

---

### 🧩 Flujo principal
1. El usuario accede a la opción “Pagar con QR”.
2. El sistema muestra el lector de código QR en pantalla.
3. El usuario escanea un código QR válido.
4. El sistema muestra el monto a pagar y los datos del comercio.
5. El usuario confirma el pago.
6. El sistema procesa la transacción.
7. El sistema muestra el mensaje “Pago realizado con éxito”.

---

### ⚠️ Flujos alternativos
- **QR inválido:** el sistema muestra un mensaje de error y no permite continuar.
- **Saldo insuficiente:** el sistema informa que no hay saldo suficiente y cancela la operación.
- **Usuario cancela:** el sistema vuelve a la pantalla inicial sin realizar el pago.

---

### ✅ Postcondiciones
- Si el pago es exitoso, el saldo del usuario se actualiza.
- La transacción queda registrada en el historial.
- Si el pago es exitoso, el saldo del usuario se actualiza.
- La transacción queda registrada en el historial.
