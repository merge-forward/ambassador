# Merge Forward — Ambassador Badges

Sitio estático para los badges de Merge Forward Ambassador, publicable en GitHub Pages.

## Estructura

```
merge-forward-badges/
├── index.html                  ← Página principal (lista de embajadores)
├── css/
│   └── styles.css              ← Todo el Design System y estilos
├── fonts/
│   ├── Gilroy-Regular.ttf
│   └── Gilroy-Bold.ttf
├── assets/
│   └── logo.png                ← Agrega aquí el logo de Merge Forward
└── ambassadors/
    └── ambassador.html         ← Plantilla de badge (duplicar por embajador)
```

## Agregar un nuevo embajador

1. Duplica `ambassadors/ambassador.html`
2. Renómbralo: `ambassadors/nombre-apellido.html`
3. Edita en el nuevo archivo:
   - `Ambassador Name` → nombre real
   - `Date issued` → fecha de emisión
   - Las iniciales `MF` del avatar → iniciales del embajador
   - El `href` del botón LinkedIn si cambia
4. En `index.html`, duplica el bloque `<a class="ambassador-card">` y actualiza nombre e `href`

## Agregar el logo

Coloca el archivo del logo en `assets/logo.png`.  
Si tu logo es SVG, cambia la extensión en `index.html` y `ambassadors/ambassador.html`.

## Publicar en GitHub Pages

```bash
git add .
git commit -m "Add ambassador badges"
git push
```

Luego en tu repo: **Settings → Pages → Branch: main → Save**  
En ~2 minutos tu sitio estará en: `https://tuusuario.github.io/nombre-repo`

## Fuentes

- **Gilroy** (Bold + Regular) — incluidas en `/fonts`
- **Barlow** — cargada desde Google Fonts (requiere conexión)
