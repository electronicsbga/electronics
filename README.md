# Electronics Parts — Tienda web + Portal administrativo

Sitio de Electronics Parts (Bucaramanga, Santander): catálogo en línea con carrito
y pedido por WhatsApp, secciones de empresa, chatbot asesor, y un portal
administrativo tipo ERP.

## Archivos

| Archivo        | Qué es |
|----------------|--------|
| `index.html`   | Tienda pública (catálogo, carrito, servicios, nosotros, preguntas, contacto, bot) |
| `admin.html`   | Portal administrativo / ERP (inventario, ventas, caja, cartera, facturas, etc.) |
| `vercel.json`  | Configuración de caché para Vercel (evita ver versiones viejas) |

## Cómo acceder

- Tienda: `https://TU-DOMINIO.vercel.app/`
- Portal: `https://TU-DOMINIO.vercel.app/admin.html` (también desde el botón "Ingresar" de la tienda)

## Desplegar en Vercel

1. Sube estos archivos a un repositorio de GitHub.
2. En vercel.com → **Add New → Project** → importa el repositorio.
3. Framework Preset: **Other**. Deja Build Command, Output Directory e Install Command **vacíos** (es un sitio estático, no necesita compilar).
4. **Deploy**. Desde ahí, cada cambio en GitHub se despliega solo.
5. Abre siempre con **Ctrl + Shift + R** tras un cambio (recarga sin caché).

## Notas importantes

- Los datos (productos, precios, pedidos, inventario) se guardan hoy en el
  navegador (**localStorage**), es decir, por dispositivo. Para que se sincronicen
  entre el celular, el computador y varios usuarios en tiempo real, hay que
  conectar **Supabase** (pendiente).
- WhatsApp del negocio: **322 398 0005**.
- El portal admin pide crear un usuario y clave la primera vez (candado local,
  no es seguridad de servidor).

## Marca

- Ciudad: Bucaramanga, Santander
- Colores: cian `#2BB8E6`, navy `#1A3A5C`, naranja `#E8622A`, rojo `#D62F2F`
