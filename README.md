# Vector2Svg

Vector2Svg es una utilidad para convertir archivos de recursos XML de Android Vector Drawable al formato SVG (Scalable Vector Graphics).

## Descripción

Android VectorDrawable es un tipo de recurso gráfico potente introducido en Android, que permite definir gráficos vectoriales complejos en archivos XML. Sin embargo, estos archivos no son directamente visibles ni editables en muchos de los programas de diseño vectorial más populares, como Adobe Illustrator.

Vector2Svg resuelve este problema convirtiendo los archivos XML de Vector Drawable en archivos SVG, que son ampliamente compatibles con muchos programas de gráficos. Esta utilidad es especialmente útil para diseñadores y desarrolladores que quieren ver o editar esta imagen vectorial utilizando su software de gráficos preferido.

## Uso

Cada argumento de la utilidad debe ser una ruta a un archivo XML de Vector Drawable. Se creará un nuevo archivo SVG en el mismo directorio que el archivo de entrada, con el mismo nombre pero con la extensión ".svg".

Aquí tienes un ejemplo de cómo utilizar la utilidad:

```bash
./vec2svg ruta/al/vectorDrawable1.xml ruta/al/vectorDrawable2.xml
```

En este ejemplo, se crearán dos archivos SVG: `ruta/al/vectorDrawable1.svg` y `ruta/al/vectorDrawable2.svg`.

## Compilación

Esta utilidad está escrita en C++ y utiliza la biblioteca tinyxml2 para analizar y crear archivos XML. Puedes compilarla utilizando CMake:

```bash
mkdir build
cd build
cmake ..
make
```

Para el compilador MSVC, ya tengo la biblioteca tinyxml2 precompilada. En este punto, puedes generar directamente la solución de Visual Studio a través de cmake y compilarla con Visual Studio.

Si tu compilador no es MSVC, o la plataforma del sistema operativo no es Windows x64, entonces asegúrate de que la biblioteca tinyxml2 esté instalada y que CMake pueda localizarla.

## Licencia

Este proyecto está licenciado bajo la Licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.