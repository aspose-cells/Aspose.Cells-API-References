---
title: "DeleteOptions.UpdateReference"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DeleteOptions-Eigenschaft. Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden"
type: docs
url: /de/net/aspose.cells/deleteoptions/updatereference/
---
## DeleteOptions.UpdateReference property

Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden.

```csharp
public bool UpdateReference { get; set; }
```

### Hinweise

Ab Version 26.7 setzen wir den Standardwert dieser Eigenschaft auf true.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteOptionsPropertyUpdateReferenceDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten und Formeln hinzufügen
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);
            worksheet.Cells["C1"].Formula = "=A1+B1";
            worksheet.Cells["A2"].PutValue(30);
            worksheet.Cells["B2"].PutValue(40);
            worksheet.Cells["C2"].Formula = "=A2+B2";

            // Erstellen Sie Löschoptionen mit UpdateReference auf true gesetzt
            DeleteOptions deleteOptions = new DeleteOptions();
            deleteOptions.UpdateReference = true;

            // Löschen Sie Spalte A, die in Formeln referenziert wird
            worksheet.Cells.DeleteColumns(0, 1, deleteOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [DeleteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


