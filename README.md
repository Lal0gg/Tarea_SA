# Tarea_SA
## Eduardo Josué González Cifuentes

#### Prompt de Ingreso
```python
Crea una aplicación web de autenticación completa con las siguientes características:
1. Un backend en Node.js con Express que incluya:
   - Registro de usuarios (email, contraseña) con almacenamiento en MongoDB.
   - Inicio de sesión con autenticación JWT.
   - Una ruta protegida que solo usuarios autenticados puedan acceder.
   - Validación de entradas para prevenir inyecciones SQL/XSS.
   - Contraseñas encriptadas con bcrypt.
2. Un frontend en React que incluya:
   - Una página de registro con formulario (email, contraseña).
   - Una página de inicio de sesión con formulario.
   - Una página protegida que muestre un mensaje de bienvenida al usuario autenticado.
3. Usa TypeScript para el backend y el frontend.
4. Incluye documentación básica en los archivos de código.
5. Asegúrate de que el código sea seguro, con manejo de errores y variables de entorno para datos sensibles (como claves JWT y conexión a MongoDB).
6. Estructura el proyecto en carpetas claras (backend, frontend).
7. Proporciona un README con instrucciones para ejecutar la aplicación.
Por favor, genera todos los archivos necesarios y organízalos en una estructura de proyecto adecuada.
```

#### La salida que se espera
```plaintext
auth-app/
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   │   └── authController.ts
│   │   ├── models/
│   │   │   └── userModel.ts
│   │   ├── routes/
│   │   │   └── authRoutes.ts
│   │   ├── middleware/
│   │   │   └── authMiddleware.ts
│   │   └── index.ts
│   ├── .env
│   ├── package.json
│   └── tsconfig.json
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Login.tsx
│   │   │   ├── Register.tsx
│   │   │   └── ProtectedPage.tsx
│   │   ├── App.tsx
│   │   ├── index.tsx
│   │   └── types.ts
│   ├── package.json
│   └── tsconfig.json
├── README.md
└── .gitignore
```

# Auth Ap
Una aplicación de autenticación simple construida con codificación de ambiente utilizando Cursor.

## Configuración
1. Clona el repositorio.
2. Backend:
   - Navega a `backend/`.
   - Ejecuta `npm install`.
   - Crea un archivo `.env` con `MONGO_URI` y `JWT_SECRET`.
   - Ejecuta `npm start`.
3. Frontend:
   - Navega a `frontend/`.
   - Ejecuta `npm install`.
   - Ejecuta `npm start`.

## Notas de Seguridad
- Utiliza bcrypt para el hash de contraseñas.
- JWT para autenticación segura.
- Validación de entradas para prevenir inyecciones XSS/SQL.

### Consideraciones de Seguridad
Encriptación de Contraseñas: El código generado usa bcrypt para encriptar contraseñas.

Validación de Entradas: Se implementan validaciones para prevenir inyecciones XSS y SQL.

JWT: Autenticación basada en tokens seguros.

Variables de Entorno: Datos sensibles como claves de API y conexión a la base de datos se almacenan en .env.

### Flujo de Trabajo con Cursor
- **Iniciar Proyecto**: Crear un nuevo proyecto en Cursor y abrir el Composer.

- **Ingresar el Prompt**: Copiar y pegar el prompt descrito anteriormente.

- **Generación de Código**: Cursor genera la estructura del proyecto y los archivos de código.

- **Revisión y Ajustes**: Revisar el código generado para asegurar que cumple con los requisitos. Usar el modo "Agent" de Cursor para realizar ajustes automáticos (por ejemplo, corregir errores o mejorar la lógica).

- **Pruebas**: Ejecutar la aplicación localmente (npm start en ambas carpetas) y probar las funcionalidades de registro, inicio de sesión y acceso a la página protegida.

- **Iteración**: Si es necesario, ingresar nuevos prompts para agregar funcionalidades, como recuperación de contraseñas o integración con proveedores de autenticación externos (Auth0).

### Ventajas del Uso de Vibe Coding
- **Rapidez:** Cursor generó una aplicación funcional en minutos, en lugar de horas o días de codificación manual.
- **Accesibilidad:** No se requiere un conocimiento profundo de TypeScript, Node.js o React para comenzar; el prompt en lenguaje natural es suficiente.
- **Flexibilidad:** Permite iterar rápidamente solicitando cambios específicos al Composer.
- **Democratización:** Usuarios no técnicos pueden crear aplicaciones funcionales con supervisión mínima.

###  Limitaciones y Precauciones
- **Revisión de Seguridad**: Aunque el prompt incluye medidas de seguridad, es crucial revisar el código generado para evitar vulnerabilidades como las descritas en (por ejemplo, claves hardcoded o configuraciones de autenticación débiles).

- **Complejidad**: Para aplicaciones más complejas, vibe coding puede requerir múltiples iteraciones y ajustes manuales.

- **Mantenimiento**: El código generado puede carecer de optimización para mantenimientos a largo plazo si no se revisa cuidadosamente.
