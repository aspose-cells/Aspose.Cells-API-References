---
title: "Enum SelectionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.SelectionType‑Enum. Der Auswahltyp der Listbox"
type: docs
url: /de/net/aspose.cells.drawing/selectiontype/
---
## SelectionType enumeration

Der Auswahlt­yp der Listbox.

```csharp
public enum SelectionType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Single | `0` | Einzel‑Auswahltyp. |
| Multi | `1` | Mehrfach‑Auswahltyp. |
| Extend | `2` | Erweiterter Auswahltyp. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassSelectionTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Listbox zum Arbeitsblatt hinzufügen
            ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 1, 5, 10);

            // Den Auswahltyp auf Einzel setzen
            listBox.SelectionType = SelectionType.Single;

            // Elemente zur Listbox hinzufügen
            listBox.SetInputRange("A1:A5", false, false);

            // Den Auswahltyp überprüfen
            Console.WriteLine("ListBox SelectionType: " + listBox.SelectionType);

            // Speichere die Arbeitsmappe
            workbook.Save("SelectionTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


