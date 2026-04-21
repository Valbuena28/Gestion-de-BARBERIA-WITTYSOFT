# Plan de Desarrollo y Definición del Problema

### 1. La Problemática
Las barberías suelen sufrir de:
1. **No-shows:** Clientes que reservan y no asisten (Pérdida de dinero).
2. **Gestión de Comisiones:** Cálculos manuales tediosos para pagar a cada barbero.
3. **Falta de Historial:** No saber qué corte se hizo el cliente la última vez.
4. **Inventario Ciego:** Pérdida de productos por falta de auditoría.

### 2. Módulos Críticos a Cubrir
* **Módulo de Citas:** Vista de calendario (Drag & Drop) y sistema de estados (Pendiente, En Silla, Completado, Cancelado).
* **Módulo de Clientes (CRM):** Galería de cortes anteriores, preferencias y frecuencia de visita.
* **Módulo de Colaboradores:** Gestión de horarios, perfiles de barberos y cálculo automático de comisiones (%).
* **Módulo de Ventas (POS):** Venta de servicios y productos físicos en una sola transacción.

### 3. Roadmap Técnico
- [ ] Sprint 1: Arquitectura Base, Database Schema & Auth.
- [ ] Sprint 2: Core de Reservas y Gestión de Barberos.
- [ ] Sprint 3: POS, Inventario y Reportes.
- [ ] Sprint 4: Implementación PWA y Notificaciones (Webhooks/n8n).
