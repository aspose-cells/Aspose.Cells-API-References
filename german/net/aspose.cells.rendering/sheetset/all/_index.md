---
title: "SheetSet.All"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SheetSet-Eigenschaft. Gibt ein Set mit allen Blättern der Arbeitsmappe in ihrer ursprünglichen Reihenfolge zurück"
type: docs
url: /de/net/aspose.cells.rendering/sheetset/all/
---
## SheetSet.All property

Erhält ein Set mit allen Blättern der Arbeitsmappe in ihrer ursprünglichen Reihenfolge.

```csharp
public static SheetSet All { get; }
```

### Beispiele

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
            // Erstelle eine Arbeitsmappe mit zwei Arbeitsblättern
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Beispieldaten in beiden Tabellenblättern festlegen
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // Speichere alle Blätter als Markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.SheetSet = SheetSet.All;
            
            workbook.Save("output.md", saveOptions);
            Console.WriteLine("All sheets saved to markdown successfully.");
        }
    }
}
```

### Siehe auch

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


