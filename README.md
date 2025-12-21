# 🛠️ System Tool Kit (STK) - v1.2

**System Tool Kit** es una sencilla herramienta de gestión, mantenimiento y control para sistemas basados en Linux (Debian/Ubuntu). Proporciona una interfaz visual intuitiva en la terminal para gestionar el hardware y la limpieza del sistema.

## 📋 Detalles de Funcionalidades

### 🧹 Súper Limpieza y Gestión de "Basura"
El script incluye un módulo de limpieza profunda que actúa sobre:
* **Caché de Paquetes:** Limpia `/var/cache/apt/archives` para liberar espacio de instaladores antiguos.
* **Residuos de Sistema:** Ejecuta `autoremove` para eliminar dependencias que ya no se usan.
* **Papelera de Usuarios:** Localiza y vacía automáticamente las carpetas de basura en `/home/*/.local/share/Trash/*`.
* **Reparación:** Intenta arreglar paquetes rotos antes de la limpieza con `apt install -f`.

### 📊 Monitor de Rendimiento en Tiempo Real 
* **CPU:** Cálculo dinámico de carga con barra de progreso visual.
* **RAM:** Visualización de memoria usada vs total en MB.
* **Temperatura:** Lectura de sensores térmicos del hardware.
* (Disponible según modelos)

### 👥 Administración de Usuarios
* Filtrado automático de usuarios reales (UID >= 1000).
* Creación y eliminación completa (incluyendo directorios `/home`).

## ⚖️ Licencia
Este proyecto está bajo la **Licencia MIT**. Eres libre de usarlo, modificarlo y distribuirlo siempre que se mantenga el crédito al autor original.

---
Desarrollado por **DanSanMar** | 2025
