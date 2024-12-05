# PandaTools

**PandaTools** es un proyecto diseñado para mejorar la experiencia de usuario en la terminal, proporcionando la capacidad de mostrar colores y formatos personalizados. Permite imprimir matrices con estilos configurables, aceptando una amplia variedad de parámetros para personalizar la presentación, incluyendo colores, estilos de texto y bordes.

**Sitio web**: https://doc-panda-panda-tools.vercel.app/


## Instalación
Para usar esta biblioteca en tu proyecto Java, sigue estos pasos:

1. Descarga la biblioteca: Puedes descargar el archivo JAR desde la sección de "Releases" de este repositorio.

2. Agrega la biblioteca a tu proyecto:
    - Si estás utilizando un IDE como Eclipse o IntelliJ, puedes agregar el archivo JAR descargado a tu proyecto como una dependencia externa
    - Si estás compilando manualmente, asegúrate de incluir el archivo JAR en tu classpath al compilar y ejecutar tu proyecto.

## Ejemplo de uso

```java
import pandatools.PandaTools;

public class Main {
    public static void main(String[] args) {
        PandaTools.println("", 0, "hello");
        PandaTools.println("ERROR", 1, "hello ERROR");
        PandaTools.println("SUCCESS", 1, "hello SUCCESS");
        PandaTools.println("WARNING", 1, "hello WARNING");
        PandaTools.println("INFO", 1, "hello INFO");
        System.out.println();

        String[][] productos = {
                {"Producto", "Precio", "Cantidad", "Total"},
                {"Manzana verde", "1.00", "5", "5.00"},
                {"Banana", "0.50", "10", "5.00"},
                {"Naranja importada china", "0.75", "8", "6.00"}
        };

        PandaTools.printMatrix(productos, "bold", "SUCCESS", "normal", "", 1);

    }
}
```

## Resultado

![image](https://github.com/user-attachments/assets/035c53a9-deb8-45e5-b6cc-9b96ad2e2eec)


@Autor: Llapapasca Montes Ronal James
