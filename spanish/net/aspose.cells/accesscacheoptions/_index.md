---
title: "Enumeración AccessCacheOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.AccessCacheOptions. Opciones de caché para el acceso a datos. Se pueden combinar múltiples opciones usando el operador ."
type: docs
url: /es/net/aspose.cells/accesscacheoptions/
---
## AccessCacheOptions enumeration

Opciones de caché para el acceso a datos. Múltiples opciones pueden combinarse usando el operador "&#x7C;".

```csharp
[Flags]
public enum AccessCacheOptions
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Sin caché para ningún acceso a datos. |
| All | `FFFFFFFFFFFFFFFF` | Aplicar todas las optimizaciones posibles para todo tipo de acceso a datos en el libro de trabajo. Todas las configuraciones y datos no deben cambiarse durante el acceso optimizado. |
| PositionAndSize | `3` | Aplicar posible optimización para obtener la posición y el tamaño del objeto (como Shape). Los ajustes de altura de fila y ancho de columna no deben modificarse durante el acceso optimizado. |
| CellsData | `9` | Aplicar posible optimización para obtener los valores de las celdas. Los datos de las celdas (datos y configuraciones de Cell, Row) no deben modificarse durante el acceso optimizado, tampoco deben crearse nuevos objetos Cell/Row (por ejemplo mediante [`Item`](../cells/item/)). |
| CellDisplay | `100086` | Aplicar posible optimización para obtener resultados relacionados con la visualización de celdas ([`DisplayStringValue`](../cell/displaystringvalue/), [`GetStyle`](../cell/getstyle/), [`GetDisplayStyle`](../cell/getdisplaystyle/), etc.). Los datos de las celdas y los objetos relacionados con el estilo (estilos de Cell/Row/Column, ancho de columna, etc.) no deben modificarse durante el acceso optimizado. |
| GetFormula | `200000` | Aplicar posible optimización para obtener fórmulas. Todos los datos y configuraciones que puedan afectar la expresión de la fórmula (nombre del Worksheet, texto del Name, columna de la tabla, etc.) no deben modificarse durante el acceso optimizado. |
| SetFormula | `400000` | Aplicar posible optimización para establecer fórmulas. Todos los datos y configuraciones que puedan afectar la expresión de la fórmula (nombre del Worksheet, texto del Name, columna de la tabla, etc.) no deben modificarse durante el acceso optimizado. |
| CalculateFormula | `800009` | Aplicar posible optimización para calcular fórmulas. Los datos de las celdas no deben modificarse durante el acceso optimizado, tampoco deben crearse nuevos objetos (Cell, Row, etc.) (por ejemplo mediante [`Item`](../cells/item/)). |
| ConditionalFormatting | `1000009` | Aplicar posible optimización para obtener el resultado de formato de los formatos condicionales. Todos los datos y configuraciones que puedan afectar el resultado de los formatos condicionales (configuraciones de los formatos condicionales, valores de celdas dependientes, etc.) no deben modificarse durante el acceso optimizado. |
| Validation | `2000009` | Aplicar posible optimización para obtener el resultado de validación. Todos los datos y configuraciones que puedan afectar el resultado de la validación (configuraciones de la validación, valores de celdas dependientes, etc.) no deben modificarse durante el acceso optimizado. |

### Observaciones

Para algunas funciones, acceder a un conjunto de datos grande requiere muchas operaciones repetidas y complejas, como búsquedas, cálculos, etc., y esas operaciones consumen mucho tiempo adicional. En situaciones comunes, todos los datos dependientes permanecen sin cambios durante el acceso, por lo que se pueden crear y utilizar cachés para mejorar el rendimiento del acceso. Con este fin, proporcionamos esta API para que el usuario pueda especificar qué tipo de acceso a datos necesita ser optimizado mediante un posible mecanismo de caché. Tenga en cuenta que, según las opciones, puede ser necesario que diferentes conjuntos de datos sean de solo lectura. Además, el rendimiento del acceso a datos depende de muchos aspectos; el uso de un mecanismo de caché no garantiza que el rendimiento mejore. En algunas situaciones, como cuando el conjunto de datos a acceder es pequeño, usar caché puede incluso consumir más tiempo porque la propia caché también requiere tiempo adicional.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AccessCacheOptionsDemo
    {
        public static void AccessCacheOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Iniciar caché de acceso con opciones específicas
            workbook.StartAccessCache(AccessCacheOptions.PositionAndSize | AccessCacheOptions.CellsData);

            // Realizar algunas operaciones que se benefician del caché
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue(i + j);
                }
            }

            // Cerrar caché de acceso
            workbook.CloseAccessCache(AccessCacheOptions.PositionAndSize | AccessCacheOptions.CellsData);

            // Guarda el libro de trabajo
            workbook.Save("AccessCacheOptionsExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


