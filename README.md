# Feliz cumpleaños, Ale · 27 🎂👻

Página de cumpleaños temática Beetlejuice. Es **un solo archivo** (`index.html`), sin dependencias ni build: se sube a GitHub Pages tal cual.

---

## 1. Pon tus archivos

```
index.html
fotos/foto1.jpg  →  foto8.jpg     (opcional, hasta 8)
video/video.mp4                    (opcional)
musica/musica.mp3                  (opcional)
```

- **Fotos:** `foto1.jpg`, `foto2.jpg`… hasta `foto8.jpg`. Si tienes menos, no pasa nada: las que falten simplemente no se muestran. (Si son `.png`, renómbralas a `.jpg` o edita el arreglo `FOTOS` al final del HTML.)
- **Video:** cualquier `.mp4` renombrado a `video.mp4`.
- **Música:** tu canción renombrada a `musica.mp3`. Empieza a sonar cuando ella toca el nombre por tercera vez (los navegadores no dejan autoplay sin toque). Hay un botón abajo a la derecha para silenciarla.
- **Fotos con leyenda:** en el `<script>`, llena `const LEYENDAS = ['nuestra primera cita', 'playa', …]`.

## 2. Cambia lo que quieras

Todo lo editable está marcado con `<!-- ✏️ ... -->` en `index.html`:

- La carta (`#carta`) y la firma `— Tuyo, siempre.`
- El nombre: busca `Ale` y `ALE` (aparece en el título, el hero y el botón del hechizo).
- El texto del hero.

## 3. Pruébala en tu compu

Doble clic a `index.html` funciona, pero para que video/música carguen bien usa un servidor local:

```powershell
python -m http.server 8000
```

Y abre http://localhost:8000

## 4. Súbela a GitHub Pages

Crea el repo en GitHub (vacío, sin README), luego en esta carpeta:

```powershell
git init
git add .
git commit -m "Feliz cumple, Ale"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/NOMBRE-DEL-REPO.git
git push -u origin main
```

Después, en GitHub: **Settings → Pages → Source: Deploy from a branch → Branch: `main` / `(root)` → Save**.

En 1–2 minutos queda en:

```
https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/
```

> Ojo: el repo debe ser **público** para que Pages funcione gratis. No subas nada que no quieras que sea público (aunque nadie va a encontrar la URL si no la compartes).

## 5. El día del cumple

Mándale el link por WhatsApp. El título y la descripción de la vista previa ya están puestos en el `<head>`.
