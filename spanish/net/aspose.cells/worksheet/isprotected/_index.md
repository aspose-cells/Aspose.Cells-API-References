---
title: "Worksheet.IsProtected"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Worksheet. Indica si la hoja de cálculo está protegida"
type: docs
url: /es/net/aspose.cells/worksheet/isprotected/
---
## Worksheet.IsProtected property

Indica si la hoja de cálculo está protegida.

```csharp
public bool IsProtected { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsProtectedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Proteger el libro de trabajo y la primera hoja de cálculo
            workbook.Protect(ProtectionType.All, "password");
            workbook.Worksheets[0].Protect(ProtectionType.All, "password", null);

            // Verifique si la hoja de cálculo está protegida
            bool isProtected = workbook.Worksheets[0].IsProtected;
            Console.WriteLine($"Worksheet is protected: {isProtected}");

            // Guarda el libro de trabajo
            workbook.Save("protected_worksheet.xlsx");

            // Cargue el libro de trabajo guardado y verifique la protección
            Workbook loadedWorkbook = new Workbook("protected_worksheet.xlsx");
            Console.WriteLine($"Loaded worksheet is protected: {loadedWorkbook.Worksheets[0].IsProtected}");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


