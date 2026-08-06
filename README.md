# Libro de Carga · Control Financiero de Estaciones de Servicio

Sistema web interactivo y multiempresa diseñado para el **Control Financiero y Carga de Reportes de Flujo de Caja** en estaciones de servicio y empresas del sector energético.

---

## 📋 ¿De qué se trata este sistema?

Este sistema permite administrar y supervisar los reportes financieros mensuales de múltiples estaciones de servicio o empresas asociadas.

### Funcionalidades Principales:

1. **Panel de Empresas (Operadores)**:
   - **Carga de Archivos Excel/CSV**: Subida drag-and-drop de archivos `.xlsx`, `.xls`, `.xlsm` y `.csv` de hasta 8 MB por período (Mes/Año).
   - **Vista Previa de Excel Interactiva**: Lectura instantánea en el navegador utilizando SheetJS con navegación por pestañas de hojas del libro.
   - **Resumen Financiero y Calculadora de Flujo Neto**: Registro de Ingresos, Gastos, Costos y Saldo en Banco/Caja con cálculo en tiempo real de Superávit o Déficit del período.
   - **Notas para Administración**: Espacio para observaciones o aclaraciones sobre el reporte mensual.
   - **Historial de Reportes**: Consulta de cargas pasadas con filtros por mes y año.

2. **Panel del Super Administrador**:
   - **Checklist de Cumplimiento**: Pantalla dedicada de control mensual con la matriz de recepción de reportes Excel, estado de datos cargados y acciones rápidas de validación.
   - **Estadísticas Visuales y Gráficos**: Barra de progreso de cumplimiento de carga (Validados %, Cargados %, Sin Cargar %) con indicadores porcentuales en tiempo real.
   - **Filtros Avanzados**: Filtrado combinado por **Empresa**, **Estado de Datos Cargados** (Todos, Sí, No), **Mes** y **Año**.
   - **Gestión de Empresas**: Módulo independiente para registrar y administrar las empresas o estaciones asociadas.
   - **Gestión de Usuarios y Accesos**: Módulo independiente para crear usuarios con su rol (`Empresa` o `Super Administrador`) y vincularlos a su empresa correspondiente.

---

## 🔑 Credenciales Grabadas en el Sistema

El sistema cuenta con datos iniciales predeterminados (*seeded*) guardados localmente. Puedes ingresar con cualquiera de las siguientes cuentas:

| Rol | Empresa / Estación | Usuario (`Username`) | Contraseña (`Password`) |
| :--- | :--- | :--- | :--- |
| **Super Administrador** | Administración General | `superadmin` | `super123` |
| **Empresa (Operador)** | AGROGASOIL, C.A. | `agrogasoil` | `agro123` |
| **Empresa (Operador)** | Centro Óptico Vicente | `covicente` | `vicente123` |
| **Empresa (Operador)** | Buena Ventura | `buenaventura` | `buenaventura123` |

> **Nota**: El Super Administrador puede crear nuevas empresas y asociarles usuarios con claves personalizadas desde los módulos **"Empresas Registradas"** y **"Usuarios y Accesos"**.

---

## 🚀 ¿Cómo Ejecutar el Sistema?

1. No requiere instalación de servidores ni bases de datos externas.
2. Abre el archivo **`libro-de-carga.html`** directamente en cualquier navegador web moderno (Google Chrome, Microsoft Edge, Firefox, Safari, Brave).
3. Toda la información y archivos cargados se almacenan de manera segura en el `localStorage` del navegador.

---

## ⚙️ Tecnologías Utilizadas

- **HTML5 & CSS3 Vanilla**: Diseño responsivo con sistema de variables CSS, glassmorphism, sombras suaves y degradados.
- **JavaScript (ES6+)**: Lógica reactiva de estado sin dependencias pesadas.
- **SheetJS (xlsx.full.min.js)**: Decodificación y renderizado de hojas de cálculo Excel directamente en el cliente.

---

## 🌐 Despliegue en Render / GitHub Pages

Para publicar este proyecto en **Render** (o GitHub Pages) como sitio web estático:

1. El archivo principal debe llamarse **`index.html`** *(ya creado en el repositorio)*.
2. En Render, crea un nuevo **Static Site**.
3. Conecta tu repositorio de GitHub.
4. Configuración en Render:
   - **Build Command**: *(Dejar vacío)*.
   - **Publish Directory**: `.` *(Raíz del proyecto)*.
5. Render desplegará la aplicación web de inmediato sin errores 404.
