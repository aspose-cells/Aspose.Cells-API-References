---
title: "Worksheet.AllowEditRanges"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Worksheet. Obtiene la colección de rangos de edición permitida en la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/alloweditranges/
---
## Worksheet.AllowEditRanges property

Obtiene la colección de rangos de edición permitidos en la hoja de cálculo.

```csharp
public ProtectedRangeCollection AllowEditRanges { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyAllowEditRangesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un rango de edición permitida
            int index = worksheet.AllowEditRanges.Add("r1", 0, 0, 1, 1);
            ProtectedRange range = worksheet.AllowEditRanges[index];
            range.Password = "password123";

            // Proteger la hoja de cálculo
            worksheet.Protect(ProtectionType.All);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");

            // Cargar el libro de trabajo guardado para verificar
            Workbook verifyWorkbook = new Workbook("output.xlsx");
            ProtectedRange verifyRange = verifyWorkbook.Worksheets[0].AllowEditRanges[0];
            Console.WriteLine("Is protected with password: " + verifyRange.IsProtectedWithPassword);
        }
    }
}
```

### Ver también

* class [ProtectedRangeCollection](../../protectedrangecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


