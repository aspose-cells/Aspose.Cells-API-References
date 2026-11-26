---
title: "PasteOptions.PasteType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PasteOptions. El tipo de pegado especial"
type: docs
url: /es/net/aspose.cells/pasteoptions/pastetype/
---
## PasteOptions.PasteType property

El tipo de pegado especial.

```csharp
public PasteType PasteType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyPasteTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer valor de origen
            worksheet.Cells["A1"].PutValue("SourceValue");

            // Crear rangos con nombres de tipo totalmente calificados
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1");
            Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("B1:D3");

            // Copiar con PasteType.All
            targetRange.Copy(sourceRange, new PasteOptions() { PasteType = PasteType.All });

            // Mostrar resultados
            Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue);
            Console.WriteLine("B1: " + worksheet.Cells["B1"].StringValue);
            Console.WriteLine("C2: " + worksheet.Cells["C2"].StringValue);
            Console.WriteLine("D3: " + worksheet.Cells["D3"].StringValue);
        }
    }
}
```

### Ver también

* enum [PasteType](../../pastetype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


