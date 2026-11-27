---
title: "DeleteBlankOptions.DrawingsAsBlank"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DeleteBlankOptions egenskap. Anger om ritningsrelaterade objekt såsom bild, form, diagram... ska betraktas som tomma. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells/deleteblankoptions/drawingsasblank/
---
## DeleteBlankOptions.DrawingsAsBlank property

Anger om ritningsrelaterade objekt såsom bild, form, diagram... ska betraktas som tomma. Standardvärdet är true.

```csharp
public bool DrawingsAsBlank { get; set; }
```

### Anmärkningar

När denna egenskap sätts till false kommer alla rader/kolumner som täcks av ritningsobjekt inte att betraktas som tomma och kommer inte att tas bort.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyDrawingsAsBlankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data");
            worksheet.Cells["B1"].PutValue("");
            worksheet.Cells["B2"].PutValue("");

            // Lägg till ett ritningsobjekt för att testa beteendet för DrawingsAsBlank
            worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 50);

            // Ta bort tomma kolumner med DrawingsAsBlank = false (bevarar ritningar)
            worksheet.Cells.DeleteBlankColumns(new DeleteBlankOptions { DrawingsAsBlank = false });

            Console.WriteLine("Drawing preserved count: " + worksheet.Shapes.Count);
        }
    }
}
```

### Se även

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


