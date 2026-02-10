# 🧪 Casos de Prueba
## Pago con QR vía PIX – Mercado Pago (Brasil)

---

### 🟢 CP-01 – Pago exitoso con QR válido

**Precondiciones:**  
Usuario con sesión iniciada y saldo suficiente.

**Pasos:**
1. Abrir la aplicación Mercado Pago.
2. Seleccionar “Pagar con QR”.
3. Escanear un código QR válido.
4. Visualizar monto y datos del comercio.
5. Confirmar el pago.

**Resultado esperado:**  
El sistema procesa el pago y muestra el mensaje “Pago realizado con éxito”.

---

### 🔴 CP-02 – Código QR inválido

**Precondiciones:**  
Usuario con sesión iniciada.

**Pasos:**
1. Abrir la aplicación Mercado Pago.
2. Seleccionar “Pagar con QR”.
3. Escanear un código QR inválido.

**Resultado esperado:**  
El sistema muestra un mensaje de error indicando que el QR no es válido y no permite continuar.

---

### 🔴 CP-03 – Saldo insuficiente

**Precondiciones:**  
Usuario con sesión iniciada y saldo insuficiente.

**Pasos:**
1. Abrir la aplicación Mercado Pago.
2. Seleccionar “Pagar con QR”.
3. Escanear un código QR válido.
4. Visualizar monto y datos del comercio.
5. Confirmar el pago.

**Resultado esperado:**  
El sistema muestra un mensaje indicando saldo insuficiente y cancela la operación.

---

### 🟡 CP-04 – Usuario cancela antes de confirmar

**Precondiciones:**  
Usuario con sesión iniciada.

**Pasos:**
1. Abrir la aplicación Mercado Pago.
2. Seleccionar “Pagar con QR”.
3. Escanear un código QR válido.
4. Visualizar monto y datos del comercio.
5. Seleccionar la opción “Cancelar”.

**Resultado esperado:**  
El sistema vuelve a la pantalla inicial sin realizar el pago.

---

### 🟡 CP-05 – Intentar volver atrás después de confirmar pago

**Precondiciones:**  
Usuario con sesión iniciada y saldo suficiente.

**Pasos:**
1. Abrir la aplicación Mercado Pago.
2. Seleccionar “Pagar con QR”.
3. Escanear un código QR válido.
4. Visualizar monto y datos del comercio.
5. Confirmar el pago.
6. Intentar volver atrás.

**Resultado esperado:**  
El sistema mantiene el pago confirmado y no permite revertir la transacción desde la navegación.
