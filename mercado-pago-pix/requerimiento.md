# 📄 Requerimiento Funcional
## Pago con código QR vía PIX – Mercado Pago (Brasil)

---

### 🎯 Objetivo
Permitir que un usuario realice un pago mediante el escaneo de un código QR utilizando PIX, visualizando previamente el monto y los datos del comercio, y confirmando el pago de forma segura.

---

### 👤 Actor principal
Usuario de la aplicación Mercado Pago.

---

### 📌 Precondiciones
- El usuario tiene sesión iniciada en la aplicación.
- El usuario tiene una cuenta habilitada para pagos con PIX.
- El comercio genera un código QR.
- El dispositivo cuenta con cámara habilitada.

---

### 🧩 Flujo principal
1. El usuario selecciona la opción “Pagar con QR”.
2. El sistema muestra el lector de código QR en pantalla.
3. El usuario escanea un código QR válido.
4. El sistema muestra el monto a pagar y los datos del comercio.
5. El usuario confirma el pago.
6. El sistema procesa la transacción.
7. El sistema muestra el mensaje “Pago realizado con éxito”.

---

### ⚠️ Flujos alternativos
- **Saldo insuficiente:** el sistema informa que no hay saldo suficiente y no permite continuar con el pago.
- **QR inválido:** el sistema muestra un mensaje indicando que el código QR no es válido.
- **QR expirado:** el sistema informa que el código QR ha expirado y no permite continuar con la operación.

---

### ✅ Postcondiciones
- Si el pago es exitoso, el saldo del usuario se actualiza.
- La transacción queda registrada en el historial de movimientos.
