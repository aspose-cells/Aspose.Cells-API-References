---
title: "ListBox.IsSelected"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListBox‑Methode. Gibt an, ob das Element ausgewählt ist"
type: docs
url: /de/net/aspose.cells.drawing/listbox/isselected/
---
## ListBox.IsSelected method

Gibt an, ob das Element ausgewählt ist.

```csharp
public bool IsSelected(int itemIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| itemIndex | Int32 | Der Elementindex. |

### Rückgabewert

ob das Element ausgewählt ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxMethodIsSelectedWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Listbox zum Arbeitsblatt hinzufügen
            ListBox listBox = worksheet.Shapes.AddListBox(0, 0, 100, 100, 200, 200);

            // Setze Listenelemente über den verknüpften Zellenbereich
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            listBox.LinkedCell = "A1:A3";

            // Ein Element auswählen
            listBox.SelectedIndex = 0;

            // Überprüfen Sie den Auswahlstatus mit IsSelected und einem Int32-Parameter
            Console.WriteLine("Item 0 selected: " + listBox.IsSelected(0));
            Console.WriteLine("Item 1 selected: " + listBox.IsSelected(1));
            Console.WriteLine("Item 2 selected: " + listBox.IsSelected(2));
        }
    }
}
```

### Siehe auch

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


