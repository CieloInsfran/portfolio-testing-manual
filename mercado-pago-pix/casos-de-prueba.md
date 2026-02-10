# 🧪 Casos de Prueba
## Pago con QR vía PIX – Mercado Pago (Brasil)

---

### 🟢 CP-01 – Pago exitoso con código QR válido

**Precondiciones:**  
- Usuario con sesión iniciada.
- Usuario con saldo suficiente.

**Pasos:**
1. Abrir la aplicación Mercado Pago.
2. Seleccionar la opción “Pagar con QR”.
3. Escanear un código QR válido.
4. Verificar el monto y los datos del comercio.
5. Confirmar el pago.

**Resultado esperado:**  
El sistema procesa el pago correctamente y muestra el mensaje “Pago realizado con éxito”.

---

### 🔴 CP-02 – Pago rechazado por saldo insuficiente

**Precondiciones:**  
- Usuario con sesión iniciada.
- Usuario con saldo insuficiente.

**Pasos:**
1. Abrir la aplicación Mercado Pago.
2. Seleccionar la opción “Pagar con QR”.
3. Escanear un código QR válido.
4. Verificar el monto y los datos del comercio.
5. Confirmar el pago.

**Resultado esperado:**  
El sistema muestra un mensaje indicando saldo insuficiente y no realiza la transacción.

---

### 🔴 CP-03 – Escaneo de código QR inválido

**Precondiciones:**  
- Usuario con sesión iniciada.

**Pasos:**
1. Abrir la aplicación Mercado Pago.
2. Seleccionar la opción “Pagar con QR”.
3. Escanear un código QR inválido.

**Resultado esperado:**  
El sistema muestra un mensaje de error indicando que el código QR no es válido y no permite continuar.

---

### 🔴 CP-04 – Escaneo de código QR expirado

**Precondiciones:**  
- Usuario con sesión iniciada.

**Pasos:**
1. Abrir la aplicación Mercado Pago.
2. Seleccionar la opción “Pagar con QR”.
3. Escanear un código QR expirado.

**Resultado esperado:**  
El sistema informa que el código QR ha expirado y no permite continuar con el pago.
