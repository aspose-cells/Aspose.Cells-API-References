---
title: "Range.GetOffset"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Obtiene un rango Range por desplazamiento"
type: docs
url: /es/net/aspose.cells/range/getoffset/
---
## Range.GetOffset method

Obtiene el rango [`Range`](../) por desplazamiento.

```csharp
public Range GetOffset(int rowOffset, int columnOffset)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowOffset | Int32 | Desplazamiento de fila en este rango, basado en cero. |
| columnOffset | Int32 | Desplazamiento de columna en este rango, basado en cero. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetOffsetWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Crear rango inicial
            Aspose.Cells.Range originalRange = cells.CreateRange("A1");
            Console.WriteLine("Original Range Address: " + originalRange.Address);
            
            // Obtener rango con desplazamiento
            Aspose.Cells.Range offsetRange = originalRange.GetOffset(1, 1);
            Console.WriteLine("Offset Range Address: " + offsetRange.Address);
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


