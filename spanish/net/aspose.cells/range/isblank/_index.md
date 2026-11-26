---
title: "Range.IsBlank"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Indica si el rango contiene valores"
type: docs
url: /es/net/aspose.cells/range/isblank/
---
## Range.IsBlank method

Indica si el rango contiene valores.

```csharp
public bool IsBlank()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodIsBlankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea un rango y verifica si está vacío (debe ser verdadero)
            Aspose.Cells.Range range1 = cells.CreateRange("A1:C10");
            Console.WriteLine("Range A1:C10 is blank: " + range1.IsBlank());

            // Coloca un valor en una celda y verifica de nuevo (debe ser falso)
            cells["B2"].PutValue("Test");
            Aspose.Cells.Range range2 = cells.CreateRange("A1:C10");
            Console.WriteLine("Range A1:C10 is blank after adding value: " + range2.IsBlank());
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


