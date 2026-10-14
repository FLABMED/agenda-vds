# Agenda pública · Fundación LAB en VDS 2026

Agenda de Fundación LAB en Valencia Digital Summit 2026 (21 y 22 de octubre), publicada con GitHub Pages.

- Página completa: `https://flabmed.github.io/agenda-vds/`
- Versión para incrustar (sin banner, altura automática): `https://flabmed.github.io/agenda-vds/?embed=1`

## Código para incrustar en otra web

```html
<iframe id="agenda-flab-vds"
  src="https://flabmed.github.io/agenda-vds/?embed=1"
  title="Agenda de Fundación LAB en VDS 2026"
  style="width:100%;border:0;min-height:900px" loading="lazy"></iframe>
<script>
  window.addEventListener("message", function (e) {
    if (e.origin !== "https://flabmed.github.io") return;
    if (e.data && e.data.type === "flab-agenda-height") {
      document.getElementById("agenda-flab-vds").style.height = e.data.height + "px";
    }
  });
</script>
```

Si el gestor de la web no permite `<script>`, basta con el `<iframe>` y una altura fija (por ejemplo `height="1600"`).

## Archivos

- `index.html`: la agenda (datos, diseño y lógica).
- `img/`: fondo del banner, logo de Fundación LAB y plano del recinto.
