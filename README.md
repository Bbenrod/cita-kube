# Cita-Kube

**Cita-Kube** es una aplicación que gestiona citas médicas de forma eficiente y escalable, usando **microservicios** y **Kubernetes**. El sistema está diseñado para ser flexible, permitiendo que médicos, recepcionistas y pacientes interactúen en tiempo real con notificaciones de estado de citas.

## 🚀 Características

- **Microservicios**: Los servicios están desacoplados, facilitando la escalabilidad y el mantenimiento.
- **Notificaciones en tiempo real**: Los pacientes reciben actualizaciones de sus citas mediante WebSockets.
- **Docker**: Cada microservicio está contenido en su propia imagen Docker para fácil despliegue.
- **Kubernetes**: El sistema está listo para ser desplegado en un clúster de Kubernetes.
- **Fases del Proyecto**:
  - Fase 1: Microservicios básicos con APIs REST.
  - Fase 2: Dockerización y comunicación entre microservicios.
  - Fase 3: Añadir WebSocket para notificaciones en tiempo real.
  - Fase 4: Frontend básico para médicos, recepcionistas y pacientes.
  - Fase 5: CI/CD con GitHub Actions.
  - Fase 6: Despliegue completo en Kubernetes.

## 🏗️ Estructura del Proyecto

```plaintext
cita-kube/
├── services/
│ ├── auth/ # Microservicio de autenticación
│ ├── appointments/ # Microservicio para gestión de citas
│ └── realtime/ # Microservicio para notificaciones en tiempo real
├── apps/
│ ├── patient/ # Interfaz del paciente
│ ├── doctor/ # Interfaz del médico
│ └── receptionist/ # Interfaz de la recepcionista
├── infra/
│ └── docker/ # Configuración Docker (Docker Compose)
├── docs/ # Documentación adicional del proyecto
├── tests/ # Tests unitarios y de integración
├── .gitignore
├── LICENSE
└── README.md
```

## 📜 Guía de Instalación

1. **Clona el repositorio**:

   ```bash
   git clone https://github.com/tuusuario/cita-kube.git
   cd cita-kube
   ```

2. **Configura el entorno**:

   Crea un archivo `.env` basado en `.env.example` y configura tus variables de entorno (si es necesario).

3. **Levanta los microservicios con Docker**:

   Usa el siguiente comando para levantar los microservicios y la base de datos de desarrollo:

   ```bash
   docker-compose up --build
   ```

4. **Accede a la aplicación**:

   Los servicios deberían estar disponibles en `localhost:3000` para el backend. Puedes empezar a interactuar con las APIs de cada servicio desde ahí.

## 🤝 Contribuciones

¡Las contribuciones son bienvenidas! Para colaborar:

1. Haz un fork del repositorio.
2. Crea una nueva rama para tu funcionalidad o corrección.
3. Envía un pull request describiendo tus cambios.

Para más detalles, consulta [CONTRIBUTING.md](CONTRIBUTING.md).

## 💡 Roadmap

1. **Fase 1**: Microservicios básicos.
2. **Fase 2**: Dockerización y comunicación entre microservicios.
3. **Fase 3**: Notificaciones en tiempo real.
4. **Fase 4**: Frontend para cada rol.
5. **Fase 5**: CI/CD con GitHub Actions.
6. **Fase 6**: Despliegue en Kubernetes.

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Para más detalles, revisa el archivo [LICENSE](LICENSE).

> **Advertencia**: Este texto fue generado con la ayuda de ChatGPT.
