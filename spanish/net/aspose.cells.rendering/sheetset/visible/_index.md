---
title: "SheetSet.Visible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SheetSet. Obtiene un conjunto con las hojas visibles del libro de trabajo en su orden original"
type: docs
url: /es/net/aspose.cells.rendering/sheetset/visible/
---
## SheetSet.Visible property

Obtiene un conjunto con las hojas visibles del libro de trabajo en su orden original.

```csharp
public static SheetSet Visible { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyVisibleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con dos hojas de cálculo
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Ocultar la segunda hoja de cálculo
            workbook.Worksheets[1].IsVisible = false;

            // Configurar opciones de guardado para exportar solo las hojas visibles
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                SheetSet = SheetSet.Visible
            };

            // Guardar el libro de trabajo (solo se exportará la hoja visible)
            workbook.Save("VisibleSheetsOnly.pptx", saveOptions);

            Console.WriteLine("Workbook saved with only visible sheets exported.");
        }
    }
}
```

### Ver también

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


