---
title: "Enumeración ParameterType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.ParameterType. Representa todos los tipos de parámetros o el tipo de valor de retorno de una función"
type: docs
url: /es/net/aspose.cells/parametertype/
---
## ParameterType enumeration

Representa el tipo de todos los parámetros o el tipo de valor de retorno de la función.

```csharp
public enum ParameterType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Reference | `0` |  |
| Value | `1` |  |
| Array | `2` |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ParameterTypeDemo
    {
        public static void ParameterTypeExample()
        {
            // Crear un libro de trabajo y una hoja de cálculo para demostrar el uso
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ejemplo de uso de la enumeración ParameterType en una función de fórmula
            // Supongamos que estamos definiendo una función personalizada con tipos de parámetros específicos

            // Definir una matriz de tipos de parámetros
            ParameterType[] parameterTypes = new ParameterType[]
            {
                ParameterType.Reference,
                ParameterType.Value,
                ParameterType.Array
            };

            // Función de ejemplo que utiliza estos tipos de parámetros
            // Por ejemplo, establecer una función personalizada hipotética con tipos de parámetros definidos
            // (Nota: El manejo de funciones personalizadas dependería de las capacidades de la API de Aspose.Cells)

            // Guardar el libro de trabajo para demostrar los cambios
            workbook.Save("ParameterTypeExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


