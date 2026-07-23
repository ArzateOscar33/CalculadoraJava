# Calculadora de escritorio en Java

Aplicación de escritorio desarrollada en **Java con Swing** que permite realizar operaciones matemáticas básicas mediante una interfaz gráfica.

Este proyecto fue creado como práctica de programación para aprender sobre manejo de eventos, interfaces gráficas, estados internos, métodos reutilizables y controles mediante teclado.

## Características

* Suma, resta, multiplicación y división.
* Operaciones encadenadas.
* Ejecución de resultados mediante el botón `=`.
* Uso de números enteros y resultados decimales.
* Eliminación visual del `.0` cuando el resultado es entero.
* Validación de división entre cero.
* Reinicio completo de la operación mediante el botón `C`.
* Compatibilidad con el teclado normal.
* Compatibilidad con el teclado numérico.
* Simulación visual de los botones al utilizar el teclado.

## Tecnologías utilizadas

* Java 21
* Java Swing
* Apache NetBeans
* Apache Ant
* Git y GitHub

## Controles

La calculadora puede utilizarse mediante los botones de la interfaz o con el teclado físico.

| Tecla            | Acción                          |
| ---------------- | ------------------------------- |
| `0` a `9`        | Introducir números              |
| `+`              | Sumar                           |
| `-`              | Restar                          |
| `*`              | Multiplicar                     |
| `/`              | Dividir                         |
| `=`              | Obtener resultado               |
| `Enter`          | Obtener resultado               |
| `Escape`         | Limpiar la calculadora          |
| Teclado numérico | Introducir números y operadores |

## Funcionamiento interno

La calculadora administra su estado mediante cuatro variables principales:

* `entradaActual`: almacena como texto el número que está escribiendo el usuario.
* `acumulado`: conserva el resultado confirmado de las operaciones.
* `operador`: almacena el operador matemático pendiente.
* `bandera`: determina si el siguiente dígito debe comenzar una entrada nueva.

La lógica está dividida en métodos reutilizables:

* `procesarNumero()`: construye la entrada numérica.
* `procesarOperador()`: procesa operaciones y resultados encadenados.
* `procesarResultado()`: confirma la operación al presionar `=`.
* `formatearNumero()`: elimina el `.0` cuando el resultado es entero.
* `configurarTeclado()`: relaciona las teclas físicas con los botones.
* `asociarTecla()`: reutiliza las acciones existentes de cada botón.

Esta estructura permite que los clics del mouse y las teclas físicas utilicen la misma lógica interna.

## Ejemplo de uso

```text
Entrada:  25 + 5 =
Resultado: 30
```

```text
Entrada:  10 / 4 =
Resultado: 2.5
```

También pueden realizarse operaciones encadenadas:

```text
5 + 3 - 2 = 6
```

## Requisitos

Para abrir y ejecutar el proyecto se necesita:

* JDK 21 o posterior.
* Apache NetBeans.
* Git, únicamente si se desea clonar el repositorio.

## Instalación

Clona el repositorio:

```bash
git clone https://github.com/ArzateOscar33/CalculadoraJava.git
```

Después:

1. Abre Apache NetBeans.
2. Selecciona **File → Open Project**.
3. Busca la carpeta `CalculadoraJava`.
4. Verifica que `calculadora.Pantalla` sea la clase principal.
5. Ejecuta el proyecto.

## Aprendizajes obtenidos

Durante el desarrollo de este proyecto se practicaron los siguientes conceptos:

* Creación de interfaces gráficas con Swing.
* Programación orientada a eventos.
* Manejo del estado de una aplicación.
* Creación y reutilización de métodos.
* Conversión entre `String` y `double`.
* Uso de estructuras condicionales.
* Uso de expresiones `switch`.
* Validación de errores.
* Manejo de eventos del teclado.
* Uso de Git y GitHub para control de versiones.

## Posibles mejoras

* Agregar entrada manual de números decimales.
* Implementar borrado mediante `Backspace`.
* Agregar cambio de signo positivo y negativo.
* Incorporar porcentajes.
* Mostrar un historial de operaciones.
* Agregar memoria matemática.
* Crear pruebas unitarias.
* Mejorar el diseño visual de la interfaz.
* Generar un instalador o ejecutable distribuible.

## Autor

Desarrollado por **Oscar Arzate**.

GitHub: **@ArzateOscar33**

---

Este proyecto fue desarrollado con fines educativos y como parte de mi proceso de aprendizaje en Java.
