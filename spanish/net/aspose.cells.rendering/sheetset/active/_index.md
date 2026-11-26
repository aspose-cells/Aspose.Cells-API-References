---
title: "SheetSet.Active"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SheetSet. Obtiene un conjunto con la hoja activa del libro de trabajo"
type: docs
url: /es/net/aspose.cells.rendering/sheetset/active/
---
## SheetSet.Active property

Obtiene un conjunto con la hoja activa del libro de trabajo.

```csharp
public static SheetSet Active { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyActiveDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con dos hojas de cálculo
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // Establece la segunda hoja de cálculo como activa
            workbook.Worksheets.ActiveSheetIndex = 1;

            // Agrega datos a ambas hojas de cálculo
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Active Sheet Data");

            // Crea opciones de guardado PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Guarda solo la hoja activa
            pdfSaveOptions.SheetSet = SheetSet.Active;
            workbook.Save("ActiveSheetOnly.pdf", pdfSaveOptions);

            // Guarda todas las hojas para comparación
            pdfSaveOptions.SheetSet = SheetSet.All;
            workbook.Save("AllSheets.pdf", pdfSaveOptions);
        }
    }
}
```

### Ver también

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


