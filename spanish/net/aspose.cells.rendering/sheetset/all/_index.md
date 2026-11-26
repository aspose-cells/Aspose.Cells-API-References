---
title: "SheetSet.All"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SheetSet. Obtiene un conjunto con todas las hojas del libro de trabajo en su orden original"
type: docs
url: /es/net/aspose.cells.rendering/sheetset/all/
---
## SheetSet.All property

Obtiene un conjunto con todas las hojas del libro de trabajo en su orden original.

```csharp
public static SheetSet All { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyAllDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con dos hojas de cálculo
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Establezca algunos datos de muestra en ambas hojas
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // Guardar todas las hojas en markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.SheetSet = SheetSet.All;
            
            workbook.Save("output.md", saveOptions);
            Console.WriteLine("All sheets saved to markdown successfully.");
        }
    }
}
```

### Ver también

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


