# ✨ Swup – Transitions magiques entre pages

Swup est une petite librairie JavaScript qui permet de faire des **transitions fluides entre les pages** d’un site, sans rechargement complet. Idéal pour un effet SPA sans framework 💫

---

## 🚀 Installation

```bash
# Avec npm
npm install swup
```

```html
<!-- Ou en CDN -->
<script src="https://unpkg.com/swup@4"></script>
```

---

## 🧩 Structure HTML de base

```html
<!DOCTYPE html>
<html lang="fr">
  <head>
    <meta charset="UTF-8" />
    <title>Mon super site</title>
  </head>
  <body>
    <div id="swup">
      <!-- Ton contenu qui change d'une page à l'autre -->
    </div>

    <script src="https://unpkg.com/swup@4"></script>
    <script>
      const swup = new Swup();
    </script>
  </body>
</html>
```

---

## 🎨 Ajouter une transition

```css
html.is-animating .transition-fade {
  opacity: 0;
  transition: opacity 0.4s ease;
}

html.is-leaving .transition-fade {
  opacity: 1;
}

.transition-fade {
  opacity: 1;
  transition: opacity 0.4s ease;
}
```

---

## 🧪 Test rapide

Crée 2 pages HTML avec le même `#swup`, ajoute quelques liens entre elles, et... c’est magique 🪄

---

## 🔌 Plugins utiles

```bash
npm install @swup/head-plugin
```

```js
import Swup from 'swup';
import SwupHeadPlugin from '@swup/head-plugin';

const swup = new Swup({
  plugins: [new SwupHeadPlugin()]
});
```

---

## 📚 Liens utiles

- Site officiel : https://swup.dev  
- GitHub : https://github.com/swup/swup

---

🧙‍♂️ Que la magie des transitions soit avec toi.