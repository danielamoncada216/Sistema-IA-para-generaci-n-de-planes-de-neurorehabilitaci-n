# NeuroFisio IA — Guía de instalación

## ¿Qué es esto?
Una aplicación web para generar planes de tratamiento fisioterapéutico neurológico basados en evidencia científica, usando inteligencia artificial.

---

## Paso 1 — Crea una cuenta en Vercel (gratis)
1. Ve a **https://vercel.com**
2. Haz clic en **"Sign Up"**
3. Regístrate con tu correo o cuenta de Google

---

## Paso 2 — Crea una cuenta en GitHub (gratis)
1. Ve a **https://github.com**
2. Haz clic en **"Sign up"**
3. Regístrate con tu correo
4. Crea un repositorio nuevo llamado `neurofisio-ia`
5. Sube los archivos de esta carpeta a ese repositorio

---

## Paso 3 — Obtén tu clave de la API de Anthropic
1. Ve a **https://console.anthropic.com**
2. Crea una cuenta
3. Ve a **"API Keys"** y crea una nueva clave
4. Cópiala — la necesitarás en el siguiente paso

---

## Paso 4 — Despliega en Vercel
1. En Vercel, haz clic en **"Add New Project"**
2. Selecciona tu repositorio `neurofisio-ia` de GitHub
3. Antes de hacer clic en "Deploy", ve a **"Environment Variables"**
4. Agrega esta variable:
   - **Nombre:** `ANTHROPIC_API_KEY`
   - **Valor:** [pega aquí tu clave de Anthropic]
5. Haz clic en **"Deploy"**

¡Listo! Vercel te dará una URL pública como `neurofisio-ia.vercel.app`

---

## ¿Cuánto cuesta?
- **Vercel:** Gratis para uso moderado (plan Hobby)
- **GitHub:** Gratis
- **Anthropic API:** Se paga por uso. Cada plan generado cuesta aproximadamente **$0.01 - $0.03 USD** (menos de $0.10 COP por plan)
  - Para una clínica que genera 50 planes/mes: aproximadamente **$1.50 USD/mes**

---

## Estructura del proyecto
```
neurofisio-ia/
├── api/
│   └── generar-plan.js    ← Servidor que conecta con Anthropic (no tocar)
├── public/
│   └── index.html         ← La aplicación web (interfaz)
├── vercel.json            ← Configuración de Vercel (no tocar)
└── README.md              ← Esta guía
```

---

## Soporte
Si tienes dudas en algún paso, el equipo de soporte de Vercel tiene chat en vivo.
Para preguntas sobre la API: https://docs.anthropic.com
