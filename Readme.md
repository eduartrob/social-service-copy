# Social Service (PostgreSQL Version)

Este servicio gestiona las publicaciones, comentarios, likes y perfiles de usuarios de la plataforma AURA. Esta es una versión migrada específicamente para usar **PostgreSQL**.

## 🚀 Inicio Rápido

Para instalar dependencias, configurar la base de datos automáticamente y arrancar el servidor, ejecuta el script único:

```bash
./setup_and_run.sh
```

Este script se encargará de:
1. Instalar dependencias (`npm install`)
2. Crear el usuario de BD `social_service_pg_user`
3. Crear la base de datos `social_service_pg_db`
4. Iniciar el servidor (`npm run dev`)

---

## 🛠 Configuración Manual

Si prefieres hacerlo manualmente:

### 1. Requisitos
- Node.js >= 16
- PostgreSQL instalado y corriendo

### 2. Instalación
```bash
npm install
```

### 3. Base de Datos
Asegúrate de que PostgreSQL tenga un usuario y base de datos que coincidan con el archivo `.env`.

**Credenciales por defecto (.env):**
- **User:** `social_service_pg_user`
- **Pass:** `social_service_secure_pass`
- **DB:** `social_service_pg_db`

### 4. Ejecución
```bash
npm run dev
```

---

## 📂 Estructura del Proyecto

```
social-service-copy/
├── src/                # Código fuente (Controllers, Services, Models)
├── docs/               # Documentación técnica y scripts de legado
├── setup_and_run.sh    # Script principal de instalación/ejecución
├── .env                # Configuración de entorno
└── package.json        # Dependencias (pg, sequelize, etc.)
```

## 📝 Documentación Adicional
Puedes encontrar documentación detallada sobre la arquitectura y la API en la carpeta `docs/`.