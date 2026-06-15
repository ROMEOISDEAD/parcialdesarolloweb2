# parcialdesarolloweb2
Sistema de Gestion de Eventos con Ticketing
Proyecto Final - Desarrollo de Aplicaciones Web II
 
========================================
REQUISITO
========================================
Node.js version 22 o superior.
Verificar con: node --version
 
========================================
COMO EJECUTAR
========================================
1. npm install
2. npm run seed
3. npm start
 
Abrir en el navegador: http://localhost:3000
 
El paso 2 solo se corre una vez (crea la base de datos con datos de prueba).
 
========================================
CREDENCIALES DE PRUEBA
========================================
Admin:   admin@eventos.com   / admin123
Cliente: cliente@eventos.com / cliente123
 
========================================
LO QUE HACE EL SISTEMA
========================================
- Registro e inicio de sesion con JWT
- Roles: admin puede crear/editar/eliminar eventos, el cliente solo compra
- Compra de tickets y reserva temporal (10 minutos)
- Control de capacidad por evento
- Rate limiting: maximo 5 intentos de login cada 15 minutos
- Headers de seguridad con Helmet (OWASP)
- Validacion de entradas en todos los endpoints
 
========================================
NOTAS
========================================
- No requiere instalar PostgreSQL ni ningun servidor externo.
- Si se quiere reiniciar los datos: borrar database.sqlite y correr npm run seed de nuevo.
 
