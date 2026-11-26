---
title: "Interfaz ICustomParser"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Interfaz Aspose.Cells.ICustomParser. Permite a los usuarios agregar su analizador de valores personalizado para convertir valores de cadena a otros objetos de valor de celda adecuados"
type: docs
url: /es/net/aspose.cells/icustomparser/
---
## ICustomParser interface

Permite a los usuarios agregar su analizador de valores personalizado para convertir valores de cadena a otro objeto de valor de celda adecuado.

```csharp
public interface ICustomParser
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetFormat](../../aspose.cells/icustomparser/getformat/)() | Obtiene el patrón de formato correspondiente al valor analizado por la última invocación de [`ParseObject`](./parseobject/). |
| [ParseObject](../../aspose.cells/icustomparser/parseobject/)(string) | Analiza la cadena dada a un objeto de valor adecuado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICustomParserDemo
    {
        public static void ICustomParserExample()
        {
            // Implementación de analizador personalizado
            ICustomParser customParser = new CustomParser();

            // Ejemplo de uso del método ParseObject
            string valueToParse = "123.45";
            object parsedValue = customParser.ParseObject(valueToParse);
            Console.WriteLine($"Parsed Value: {parsedValue}");

            // Ejemplo de uso del método GetFormat
            string format = customParser.GetFormat();
            Console.WriteLine($"Format: {format}");
        }
    }

    // Implementación personalizada de ICustomParser
    public class CustomParser : ICustomParser
    {
        private string lastFormat;

        public object ParseObject(string value)
        {
            // Lógica de análisis de ejemplo
            if (double.TryParse(value, out double result))
            {
                lastFormat = "0.00"; // Example format
                return result;
            }
            lastFormat = null;
            return null;
        }

        public string GetFormat()
        {
            return lastFormat;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


