---
title: "DeleteBlankOptions.EmptyStringAsBlank"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DeleteBlankOptions-Eigenschaft. Gibt an, ob eine Zelle als leer betrachtet wird, wenn ihr Wert ein leerer String ist. Standardwert ist true"
type: docs
url: /de/net/aspose.cells/deleteblankoptions/emptystringasblank/
---
## DeleteBlankOptions.EmptyStringAsBlank property

Gibt an, ob eine Zelle als leer betrachtet wird, wenn ihr Wert ein leerer String ist. Standardwert ist true.

```csharp
public bool EmptyStringAsBlank { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEmptyStringAsBlankDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Arbeitsblatt mit Daten einschließlich leerer Zeichenketten füllen
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue("");
            worksheet.Cells["A3"].PutValue("More Data");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["A5"].PutValue("Even More Data");

            // DeleteBlankOptions mit EmptyStringAsBlank auf true konfigurieren
            DeleteBlankOptions options = new DeleteBlankOptions
            {
                EmptyStringAsBlank = true
            };

            // Zeilen löschen, die leere Zeichenketten enthalten (als leer behandelt)
            worksheet.Cells.DeleteBlankRows(options);

            // Ergebnis speichern
            workbook.Save("DeleteBlankOptions_EmptyStringAsBlank_Output.xlsx");
        }
    }
}
```

### Siehe auch

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


