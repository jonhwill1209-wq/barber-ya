# BarberYa Web

Aplicación Web del proyecto BarberYa.

Tecnologías previstas:

- Next
- TypeScript

## Base de datos

Requiere un `.env.local` (no se sube al repo) con al menos:

```
DATABASE_URL="postgresql://..."
SESSION_SECRET="una cadena aleatoria larga"
RESEND_API_KEY="" # opcional, sin ella se omite el envío de correos
```

Aplicar las migraciones y cargar los datos de prueba:

```
npx prisma migrate deploy
npx prisma db seed
```

Usuarios de prueba tras el seed: `admin@barberya.test` / `Admin123!` (administrador) y `henry@barberya.test` / `Barber123!` (barbero).
