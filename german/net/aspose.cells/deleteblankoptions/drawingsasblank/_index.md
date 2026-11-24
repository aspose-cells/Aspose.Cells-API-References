---
title: "DeleteBlankOptions.DrawingsAsBlank"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DeleteBlankOptions-Eigenschaft. Gibt an, ob zeichnungsbezogene Objekte wie Bild, Form, Diagramm... als leer betrachtet werden. Standardwert ist true"
type: docs
url: /de/net/aspose.cells/deleteblankoptions/drawingsasblank/
---
## DeleteBlankOptions.DrawingsAsBlank property

Gibt an, ob zeichnungsbezogene Objekte wie Bild, Form, Diagramm… als leer betrachtet werden. Standardwert ist true.

```csharp
public bool DrawingsAsBlank { get; set; }
```

### Hinweise

Wenn diese Eigenschaft auf false gesetzt wird, werden alle von Zeichenobjekten bedeckten Zeilen/Spalten nicht als leer betrachtet und nicht gelöscht.

### Beispiele

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

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data");
            worksheet.Cells["B1"].PutValue("");
            worksheet.Cells["B2"].PutValue("");

            // Fügen Sie ein Zeichenobjekt hinzu, um das Verhalten von DrawingsAsBlank zu testen
            worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 50);

            // Leere Spalten löschen mit DrawingsAsBlank = false (erhält Zeichnungen)
            worksheet.Cells.DeleteBlankColumns(new DeleteBlankOptions { DrawingsAsBlank = false });

            Console.WriteLine("Drawing preserved count: " + worksheet.Shapes.Count);
        }
    }
}
```

### Siehe auch

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


