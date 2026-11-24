---
title: "Style.IsLocked"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob eine Zelle bearbeitet werden kann oder nicht"
type: docs
url: /de/net/aspose.cells/style/islocked/
---
## Style.IsLocked property

Liest oder setzt einen Wert, der angibt, ob eine Zelle bearbeitet werden kann oder nicht.

```csharp
public bool IsLocked { get; set; }
```

### Hinweise

Das Sperren von Zellen hat keine Wirkung, wenn das Arbeitsblatt nicht geschützt ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsLockedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Setzen Sie die IsLocked-Eigenschaft für eine Zelle
            Cell cell = cells["A1"];
            Style style = cell.GetStyle();
            style.IsLocked = true;
            cell.SetStyle(style);

            // Schützen Sie das Arbeitsblatt, um das Sperren durchzusetzen
            worksheet.Protect(ProtectionType.All);

            // Überprüfen und drucken Sie den IsLocked-Status
            Console.WriteLine("Cell A1 IsLocked: " + cells["A1"].GetStyle().IsLocked);
            Console.WriteLine("Cell B1 IsLocked: " + cells["B1"].GetStyle().IsLocked);

            // Speichere die Arbeitsmappe
            workbook.Save("IsLockedDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


