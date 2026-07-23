# ⚡ SETUP — Sales Evidence AI

## Opción 1: Ejecutar localmente (RECOMENDADO)

```bash
# 1. Clonar repo (o descargar esta carpeta)
git clone <tu-repo> sales-evidence-ai
cd sales-evidence-ai

# 2. Instalar dependencias (solo una vez)
npm install

# 3. Ejecutar
npm run dev

# ✅ Listo en http://localhost:5173
```

## Opción 2: Desplegar en Vercel (1 click)

1. Sube esta carpeta a GitHub
2. Abre [vercel.com](https://vercel.com)
3. Conecta tu repo → Deploy

**¡Listo en 60 segundos!**

## Opción 3: Desplegar en Netlify

1. Sube a GitHub
2. Abre [netlify.com](https://netlify.com)
3. Conecta repo
4. Build command: `npm run build`
5. Publish directory: `dist`

## ¿Cómo agregar casos?

Edita `/public/casos.json` y agrega nuevos casos al array JSON.

**Los cambios se reflejan automáticamente sin recompilar.**

### Estructura de un caso:

```json
{
  "id": 61,
  "nombre": "Juan García",
  "profesion": "Empresario",
  "pais": "Colombia",
  "capitalInicial": "2000 USD",
  "capitalInitialUSD": 2000,
  "resultado": "Primeras ventas",
  "facturación": "25,000,000 pesos",
  "margen": "60%",
  "tiempoRecuperacion": "30 días",
  "objeciones": ["Tenía miedo", "No sabía importar"],
  "perfil": ["Empresario", "Padres"],
  "tags": ["accesorios", "aliexpress", "dropshipping"],
  "resumen": "Empresario que escaló rápidamente vendiendo accesorios.",
  "youtubeLink": "https://www.youtube.com/watch?v=...",
  "transcripcion": "Transcripción completa aquí..."
}
```

## Comandos principales

```bash
npm run dev          # Desarrollo (localhost:5173)
npm run build        # Producción (carpeta dist/)
npm run preview      # Preview del build
npm run lint         # Linter
```

## Estructura completa

```
sales-evidence-ai/
├── public/
│   └── casos.json              ← Edita aquí para agregar casos
├── src/
│   ├── components/             ← Componentes React
│   ├── styles/                 ← Estilos CSS
│   ├── App.jsx                 ← Componente principal
│   └── main.jsx                ← Entry point
├── index.html                  ← HTML base
├── package.json                ← Dependencias
├── vite.config.js              ← Config Vite
└── README.md                   ← Documentación completa
```

## Troubleshooting

### "npm: command not found"
Instala [Node.js](https://nodejs.org/) (v16+)

### "Port 5173 already in use"
```bash
npm run dev -- --port 3000
```

### "Cambios en JSON no aparecen"
Recarga el navegador (Ctrl+Shift+R)

### "Subida a GitHub"
```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin <tu-repo>
git push -u origin main
```

---

**¿Necesitas ayuda?** Lee `README.md` para documentación completa.

**¡A conquistar! 🚀**
