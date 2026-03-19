# Kiosk-Service

## Descripción

## Descripción

**Kiosk-Service** es un microservicio que gestiona la operación y funcionalidad de los kioscos de autoservicio de la plataforma. Los kioscos son terminales de atención al público ubicadas en puntos estratégicos que permiten a los afiliados y beneficiarios realizar consultas, trámites y transacciones de forma autónoma sin necesidad de asistencia presencial.

Maneja datos como:
- Gestión de transacciones en kioscos
- Control de dispositivos y terminales
- Sincronización de información en puntos de atención
- Reportes de operación de kioscos
- Autenticación y validación de usuarios en terminales
- Gestión de sesiones y seguridad en kioscos


---

## Clonar el repositorio y agregarle un nombre nuevo del nuevo proyecto

```bash
git clone https://github.com/MUTUAL-DE-SERVICIOS-AL-POLICIA/template-microservice.git nombre_nuevo-microservice
```

## Inicializar proyecto

```bash
# Entrar al repositorio clonado con el nuevo nombre del proyecto
cd nuevo_nombre_del_micro_servicio

# Elimina el origen remoto actual
git remote remove origin

# Crear el archivo .env en base al .env.template
cp .env.template .env

# Instalar las dependencias
pnpm install

# Correr proyecto en modo desarrollo
pnpm start:dev

# Crear nuevo Módulo
nest g res nombreModulo

# Para enlazar a un nuevo repositorio
git remote add origin https://github.com/tu-usuario/{nombre-kiosk-service}.git
git add .
git commit -m "Inicialización del nuevo proyecto"
git branch -M main
git push -u origin main
```