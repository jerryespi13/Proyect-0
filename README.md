# Project 0
## Información del proyecto
- Titulo:  `Información acerca de la diabetes`
- Autor:  `Jerry Ronaldo Espino Inestroza`
- Descripción: Proyecto 0 de programación web. Se basa en una página estática la cuál muestra información básica acerca de la enfermedad llamada diabetes, entre esta información podemos encontrar: cúales son los tipos de diabetes, cómo prevenirla, y cómo aplicar una inyección de insulina.
<!--- Video: [video]()-->

## Install & Dependence
- [SASS](https://sass-lang.com/)
## 🛠 Skills
- HTML
- CSS
- SASS
- Bootstrap
## Jerarquía del directorio
```
|—— css
|    |—— styles.css
|    |—— styles.css.map
|    |—— styles.scss
|—— diabete.ico
|—— imagenes
|    |—— Diabetes.jpg
|    |—— diabetes.jpg.webp
|    |—— inyeccion.jpg
|    |—— inyeccion1.jpg
|    |—— inyeccion2.jpg
|    |—— inyeccion3.jpg
|    |—— inyeccion4.jpg
|    |—— inyeccion5.jpg
|    |—— inyeccion6.jpg
|    |—— inyeccion7.jpg
|    |—— inyeccion8.jpg
|—— index.html
|—— inyeccion.html
|—— prevencion.html
|—— tratamiento.html
|—— README.md
```
## Detalles del proyecto
### Requerimientos solicitados
- [x] Tu sitio debe contener al menos 4 diferentes páginas .html, y debe ser posible entrar desde una página hasta otra siguiendo uno o más hipervínculos.
- [x] Tu sitio debe contener al menos una lista (ordenada o desordenada), al menos una tabla y al menos una imagen.
- [x] Tu sitio debe contener al menos una hoja de estilos.
- [x] Tu sitio debe usar al menos 5 diferentes propiedades CSS, y al menos 5 selectores diferentes. Debes usar el selector de #id y el de .class al menos una vez.
- [x] Tu sitio debe contener al menos un selector responsivo @media query, que debe aplicarse a pantallas más pequeñas.
 >`Este se encuentra en el archivo SASS linea 180`
- [x] Debes usar bootstrap 4 en tu sitio, para utilizar al menos un componente de bootstrap, y al menos dos columnas de bootstrap usando su grid layout.
 >`Este se encuentra en el archivo index.html linea 90`
```
<div class="row" id="grid-index">
    <div class="col-lg-6 col-md-12 col-sm-12 ">
        <table class="table">
            <thead>
                <tr>
                    <th>NIVELES DE GLUCOSA (mg/dL)</th>
                    <th>NORMAL</th>
                    <th>PREDIABETES</th>
                    <th>DIABETES</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td scope="row">AYUNAS</td>
                    <td>60 - 100</td>
                    <td>100 - 125</td>
                    <td>Mayor 126</td>
                </tr>
                <tr>
                    <td scope="row">2 HORAS DESPUÉS DE LOS ALIMENTOS</td>
                    <td>140</td>
                    <td>140 - 199</td>
                    <td>Más de 200</td>
                </tr>
            </tbody>
        </table>
        <p>Los niveles de azúcar en la sangre le permiten
            conocer si sus valores son normales, si es
            prediabético o diabético.</p>
    </div>
    <div class="col-lg-6 col-md-12 col-sm-12">
        <picture>
            <img src="./imagenes/diabetes.jpg.webp" alt="imagen glucometro">
        </picture>
    </div>
</div>
```
- [x] Tus hojas de estilo deben contener al menos una variable SCSS, al menos un ejemplo de anidamiento SCSS y al menos un uso de herencia SCSS.
>`Anidación con SASS en el archivo SASS linea 90`
```
#grid-index{
    div .table{
        width: 100%;
        text-align: left;
        td{
            background-color: #d9d9d9;
        }
        thead{
            tr :first-child{
                color: black;
            }
            tr :nth-child(2) {
                color: $color-diabete-normal;
            }
            tr :nth-child(3) {
                color: $color-prediabete;
            }
            tr :last-child {
                color: $color-diabete;
            }
        }
        tbody{
            text-align: center;
            tr :first-child {
                color: black;
                text-align: left;
            }
            tr :nth-child(2) {
                color: $color-diabete-normal;
            }
            tr :nth-child(3) {
                color: $color-prediabete;
            }
            tr :last-child {
                color: $color-diabete;
            }
        }
    }
    p{
        font-weight: bold;
        font-size: smaller;
    }
}

```
>`Herencia con SASS en el archivo SASS linea 142`
```
footer {
    @extend %topes;
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    height: 3rem;

    p{
        @extend %centrado;
        strong a{
            color: white;
        }
    }
}
```
>`Variables con SASS en el archivo SASS primeras lineas`
- [x] En README.md, incluye una breve descripción de tu proyecto, opcionalmente, que contiene cada archivo, y cualquier otra información adicional para el staff.
### Descripción de la pagina
La página esta conformada por un navbar fijo en la parte superior de la pantalla el cual es responsivo gracias a una clase de botstrap, este navbar se vuelve un menú hamburguesa en dispositivos moviles.

Contiene un footer en la parte baja de la página que contiene algunas clases CSS para darle estilo.

>`Página index.hmtl`

En esta página se muestra información a cerca de que es la diabetes, los tipos de diabetes que existen con sus respectivos sintomas y cuales son los niveles de glucosa según el tipo de diabetes.

>`Página tratamiento.hmtl`

En esta página se muestra información de algunos de los tratamientos que se deben de tomar en cuenta sobre una persona que padecie diabetes, ya sea su alimentación o tipo de medicina para cada tipo de diabetes.

>`Página prevención.hmtl`

En esta página se dan algunas recomendaciones que se deben de tomar para prevenir o retrasar el diagnostico de diabetes.


>`Página inyeccion.hmtl`

En esta página se explica paso a paso cómo administrar una inyección de insuluna, esta página contiene varias imagenes para dar una mejor referencia de lo que se esta hablando.