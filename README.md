# Event Horizon

Laboratorio interactivo de exploración espacial y gravedad relativista. La página de inicio está en `index.html`; el simulador original se conserva en `event_horizon_viaje_interactivo_hacia_un_agujero_negro.html`.

## Ejecutar localmente

Desde la raíz del repositorio:

```sh
python -m http.server 8000
```

Abre `http://localhost:8000/`. No requiere instalación de paquetes ni compilación.

## Navegación

La portada enlaza al laboratorio completo y permite abrir destinos concretos mediante el parámetro `target`:

- `?target=saturn`: Saturno.
- `?target=gargantua`: agujero negro.
- `?target=pulsar`: estrella de neutrones.

También se admiten los demás identificadores definidos en `ASTRO_TARGETS`. Si no se indica un destino o no es válido, se abre Saturno. El enlace **Inicio** del laboratorio permite regresar a la portada.

## Diseño y dependencias

La portada utiliza HTML, CSS y una ilustración SVG propia, sin JavaScript ni recursos externos. Incluye estilos adaptables, navegación con teclado y respeto por la preferencia de movimiento reducido.

El simulador conserva sus dependencias externas existentes: Tailwind CSS, Lucide, Three.js, fuentes, texturas y archivos de la NASA. Requiere conexión a Internet y un navegador con WebGL. Las representaciones visuales son ilustrativas.
