# Pequeñitos Store
React + TypeScript + Vite + Supabase + Netlify.

## Local
npm install
npm run dev

## Supabase
1. Crea un proyecto.
2. SQL Editor -> ejecuta `supabase/schema.sql`.
3. Authentication -> Users -> crea tu usuario administrador.
4. Ejecuta: `insert into public.profiles(id,role,full_name) values('UUID','admin','Sandra');`
5. Crea Storage buckets: `product-images`, `site-media`, `blog-images`.
6. Copia `.env.example` a `.env.local` y coloca URL + publishable key.

## GitHub
git init
git add .
git commit -m "Pequeñitos initial store"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/pequenitos-store.git
git push -u origin main

## Netlify
Importa el repositorio desde GitHub.
Build: `npm run build`
Publish: `dist`
Agrega las variables VITE_SUPABASE_URL y VITE_SUPABASE_PUBLISHABLE_KEY.

## Importante
El proyecto ya incluye Home, catálogo, producto, carrito, checkout, login admin, dashboard inicial, creación de producto, esquema Supabase, RLS y configuración Netlify.
La siguiente iteración debe completar Media Library, editor visual Gutenberg, edición de productos, variantes, páginas draft/published, blog, SEO dinámico, Storage policies y pagos.
