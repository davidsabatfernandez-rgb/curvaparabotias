# ÍCARO · Curva y ciclo (estático para Vercel)

Página única, sin backend. Los datos del atleta se guardan solo en el navegador de quien la usa (localStorage); no se envían a ningún servidor.
El PDF se genera en el navegador con jsPDF (se carga desde cdn.jsdelivr.net al pulsar "Descargar PDF").

## Subir a Vercel

Opción A, terminal (una vez):
    cd icaro-curva
    npx vercel@latest login      # abre el navegador para entrar en tu cuenta
    npx vercel@latest --prod     # acepta las preguntas por defecto; nombre del proyecto: icaro-curva

Opción B, web: sube esta carpeta a un repositorio de GitHub y en vercel.com → Add New → Project → Import ese repositorio.
Framework preset: "Other". Sin build command. Output directory: raíz.

## Actualizar
Sustituye index.html y vuelve a ejecutar `npx vercel@latest --prod` (o haz push al repositorio).

## Aviso
La URL de Vercel es pública para quien la tenga (no indexada). No contiene datos de atletas.
