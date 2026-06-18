# cartas 🧿

Sobres de cartas digitales del tipo **"Ábrelo cuando…"**. Mobile-first, minimalista, con motivo de nazar (ojo turco) y paleta azul Egeo + oro.

Un regalo para una relación a distancia: ella ve la colección de sobres sellados, y tú vas habilitando una carta cada día.

## Uso

Abre `index.html` en cualquier navegador. Todo (HTML, CSS, JS) está en un solo archivo.

## Habilitar cartas (lo controlas tú)

En el `<script>` de `index.html`, edita el array `unlockedLetters`. `true` desbloquea esa carta:

```js
const unlockedLetters = [
  true,   // 0: me extrañes
  false,  // 1: tengas un mal día
  false,  // 2: no puedas dormir
  false   // 3: necesites una sonrisa
];
```

Sube el cambio y, al recargar, esa carta se podrá abrir. Las selladas muestran el modal de "Aún no está sellado…".

## Personalizar

- **Nombres:** busca `Grachi` (destinataria) y `Jotace` (remitente).
- **Contenido:** edita el array `lettersData` (`title` y `content`; usa `\n` para saltos de línea).
- **Colores:** variables CSS `:root` al inicio del `<style>`.
- **Preview de WhatsApp:** etiquetas `og:` en el `<head>`.
