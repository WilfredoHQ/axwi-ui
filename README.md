# Axwi-ui

Conjunto de utilidades y algunos componentes css.

## Comenzando 🚀

_Estas instrucciones te permitirán obtener el proyecto en funcionamiento en tu máquina local para propósitos de desarrollo y pruebas._

### Instalación 🔧

- Instale los archivos fuente Sass a través de npm
  ```
  npm install --save-dev axwi-ui
  ```
  - Luego de haberlo instalado importe en su archivo de sass `@import "~axwi-ui/axwi-ui"`
- Cuando solo necesite incluir CSS compilado en su última versión, puede usar el CDN
  ```
  <link href="https://unpkg.com/axwi-ui/src/css/axwi-ui.min.css" rel="stylesheet">
  ```

### Uso 🔥

_Puedes usar las siguientes variables, clases, funciones y mixins._

1. Clases
   - `biggerTitle`
   - `[t1|t2|t3|t4|t5|t6]`
   - `[biggest|bigger|big|normal|small|smaller]`
   - `bodyFont`
   - `headingFont`
   - `[error|secondary|primary|success|accent|warning|red|pink|purple|deepPurple|indigo|blue|lightBlue|cyan|teal|green|lightGreen|lime|yellow|amber|orange|deepOrange|brown|grey|blueGrey][50|100|200|300|400|500|600|700|800|900|A100|A200|A400|A700]`
   - `bg[Error|Secondary|Primary|Success|Accent|Warning|Red|Pink|Purple|DeepPurple|Indigo|Blue|LightBlue|Cyan|Teal|Green|LightGreen|Lime|Yellow|Amber|Orange|DeepOrange|Brown|Grey|BlueGrey|surfaceBackground|commentBackground|Overlay|TextPrimary|TextSecondary|BlueLink|Transparent][50|100|200|300|400|500|600|700|800|900|A100|A200|A400|A700]`
   - `hoverBg[Error|Secondary|Primary|Success|Accent|Warning|Red|Pink|Purple|DeepPurple|Indigo|Blue|LightBlue|Cyan|Teal|Green|LightGreen|Lime|Yellow|Amber|Orange|DeepOrange|Brown|Grey|BlueGrey|surfaceBackground|commentBackground|Overlay|TextPrimary|TextSecondary|BlueLink|Transparent][50|100|200|300|400|500|600|700|800|900|A100|A200|A400|A700]`
   - `text[Error|Secondary|Primary|Success|Accent|Warning|Red|Pink|Purple|DeepPurple|Indigo|Blue|LightBlue|Cyan|Teal|Green|LightGreen|Lime|Yellow|Amber|Orange|DeepOrange|Brown|Grey|BlueGrey|surfaceBackground|commentBackground|Overlay|TextPrimary|TextSecondary|BlueLink|Transparent][50|100|200|300|400|500|600|700|800|900|A100|A200|A400|A700]`
   - `hoverText[Error|Secondary|Primary|Success|Accent|Warning|Red|Pink|Purple|DeepPurple|Indigo|Blue|LightBlue|Cyan|Teal|Green|LightGreen|Lime|Yellow|Amber|Orange|DeepOrange|Brown|Grey|BlueGrey|surfaceBackground|commentBackground|Overlay|TextPrimary|TextSecondary|BlueLink|Transparent][50|100|200|300|400|500|600|700|800|900|A100|A200|A400|A700]`
   - `[breakpoint]-z[Back|Normal|Tooltip|Fixed|Modal]`
   - `[breakpoint]-border`
   - `[breakpoint]-borderNone`
   - `[breakpoint]-border[Top|Right|Bottom|Left]`
   - `[breakpoint]-border[Top|Right|Bottom|Left]None`
   - `[breakpoint]-rounded[Full|05|1|2|3|4|5|6|7|8|9|10]`
   - `[breakpoint]-[tl|tr|br|bl]Rounded[05|1|2|3|4|5|6|7|8|9|10]`
   - `[breakpoint]-ratio[1|2|3|4]-[1|2|3|4]`
   - `[breakpoint]-ratio[16-9|9-16|21-9]`
   - `[breakpoint]-opacity[1|2|3|4|5|6|7|8|9|10]`
   - `[breakpoint]-shadow`
   - `[breakpoint]-[shadow|select|outline|list]None`
   - `[breakpoint]-cursorPointer`
   - `[breakpoint]-overflowHidden`
   - `[breakpoint]-[uppercase|lowercase|capitalize]`
   - `square`
   - `circle`
   - `scroll`
   - `Button`
     - `.is-ghost`
     - `.is-text`
     - `.is-big`
     - `.is-small`
     - `.is-tiny`
     - `.is-micro`
     - `.is-full`
   - `lightMode`
2. Variables
   1. Sass
      - `$l-unit` Unidad básica para el layout, _valor por default:_ `.5rem`
      - `$breakpoints` Breakpoints, _valor por default:_ `(s: 0, m: 640px, lg: 1024px, xl: 1440px)`
   2. Css
      - `--biggerFontSize: #{rem(28px)};`
      - `--h1FontSize: #{rem(24px)};`
      - `--h2FontSize: #{rem(20px)};`
      - `--h3FontSize: #{rem(16px)};`
      - `--normalFontSize: #{rem(15px)};`
      - `--smallFontSize: #{rem(13px)};`
      - `--smallerFontSize: #{rem(12px)};`
      - `--headingLineHeight: 1.3;`
      - `--bodyLineHeight: 1.6;`
      - `--[error|secondary|primary|success|accent|warning|red|pink|purple|deepPurple|indigo|blue|lightBlue|cyan|teal|green|lightGreen|lime|yellow|amber|orange|deepOrange|brown|grey|blueGrey][50|100|200|300|400|500|600|700|800|900|A100|A200|A400|A700]`
      - `--webWash: #18191a`
      - `--surfaceBackground: #242526`
      - `--commentBackground: #3a3b3c`
      - `--overlay: rgba(255, 255, 255, 0.1)`
      - `--textPrimary: #e4e6eb`
      - `--textSecondary: #b0b3b8`
      - `--blueLink: #4599ff`
      - `--divider: #3e4042`
      - `--shadowColor: rgba(0, 0, 0, 0.2)`
      - `--transparent: transparent`
3. Mixins
   - `l-unit`
   - `ratio`
   - `bp-prefix($names, $property, $value, $concat)` Se usa para convetir cualquier clase en la nomenclatura de la biblioteca **breakpoint-name**
   - `from($bp)` Para tamaños mayores al breakpoint (parámetro)
   - `to($bp)` Para tamaños menores al breakpoint (parámetro)
4. Funciones
   - `color-yiq($color)`
   - `rem($px)` Esta función convierte un número en px a rem
   - `get-bp($bp)` Obtiene un breakpoint del core
   - `str-capitalize($string)` Capitaliza un string
   - `str-initials($string)` Extrae las primeras letras de un string escrito en kebab-case ejemplo: hola-mundo => hm

## Despliegue 📦

1. In process...

## Licencia 📄

Este proyecto está bajo la Licencia (GPL-2.0) - mira el archivo [LICENSE](LICENSE) para detalles.
