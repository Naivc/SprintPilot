# SprintPilot

## 📋 Introducción al Proyecto

SprintPilot es una aplicación web moderna diseñada para la gestión de requisitos y tareas de sprint. Construida con Node.js y Express, esta aplicación permite a los equipos de desarrollo organizar, priorizar y dar seguimiento a los requisitos del proyecto de manera eficiente.

### Tecnologías Utilizadas

- **Backend**: Node.js, Express 5
- **Base de Datos**: MongoDB con Mongoose
- **Motor de Plantillas**: EJS
- **Seguridad**: Helmet
- **Logging**: Morgan
- **Herramientas de Desarrollo**: Nodemon, ESLint, Jest

---

## 🚀 Tutorial de Inicio

### Requisitos Previos

Antes de comenzar, asegúrate de tener instalado:

- **Node.js** (versión 14 o superior) - [Descargar](https://nodejs.org/)
- **MongoDB** (versión 4.4 o superior) - [Descargar](https://www.mongodb.com/try/download/community)
- **Git** - [Descargar](https://git-scm.com/)

### Paso 1: Clonar el Repositorio

```bash
git clone https://github.com/Naivc/SprintPilot.git
cd SprintPilot
```

### Paso 2: Instalar Dependencias

Instala todas las dependencias necesarias del proyecto:

```bash
npm install
```

### Paso 3: Configurar Variables de Entorno

Crea un archivo `.env` en la raíz del proyecto con las siguientes variables:

```env
PORT=3000
MONGODB_URI=mongodb://localhost:27017/sprintpilot
NODE_ENV=development
```

**Nota**: Ajusta `MONGODB_URI` según tu configuración de MongoDB.

### Paso 4: Iniciar MongoDB

Asegúrate de que MongoDB esté ejecutándose en tu sistema:

**Windows**:
```bash
# Si MongoDB está instalado como servicio
net start MongoDB
```

**macOS/Linux**:
```bash
# Usando Homebrew (macOS)
brew services start mongodb-community

# O manualmente
mongod --dbpath /ruta/a/tu/directorio/de/datos
```

### Paso 5: Poblar la Base de Datos (Opcional)

Para cargar datos de ejemplo en la base de datos:

```bash
npm run seed
```

Este comando creará requisitos de ejemplo en tu base de datos.

### Paso 6: Iniciar la Aplicación

**Modo Producción**:
```bash
npm start
```

**Modo Desarrollo** (con recarga automática):
```bash
npm run dev
```

### Paso 7: Acceder a la Aplicación

Abre tu navegador web y navega a:

```
http://localhost:3000
```

¡Deberías ver la interfaz de SprintPilot en funcionamiento!

## 📝 Scripts Disponibles

| Script | Comando | Descripción |
|--------|---------|-------------|
| Iniciar | `npm start` | Inicia el servidor en modo producción |
| Desarrollo | `npm run dev` | Inicia con Nodemon (recarga automática) |
| Poblar DB | `npm run seed` | Carga datos de ejemplo en MongoDB |
| Lint JS | `npm run lint:js` | Ejecuta ESLint en archivos JavaScript |
| Lint EJS | `npm run lint:ejs` | Ejecuta linting en plantillas EJS |
