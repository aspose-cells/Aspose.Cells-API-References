---
title: "AutoFilter.Range"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AutoFilter. Representa el rango al que se aplica el AutoFilter especificado"
type: docs
url: /es/net/aspose.cells/autofilter/range/
---
## AutoFilter.Range property

Representa el rango al que se aplica el AutoFilter especificado.

```csharp
public string Range { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["A5"].PutValue("Item4");

            // Aplicar auto filtro al rango A1:A5
            sheet.AutoFilter.Range = "A1:A5";

            // Mostrar el rango del auto filtro
            Console.WriteLine("AutoFilter Range: " + sheet.AutoFilter.Range);

            // Guarda el libro de trabajo
            workbook.Save("AutoFilterRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


