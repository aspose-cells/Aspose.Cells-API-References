---
title: "ShapeCollection.UpdateSelectedValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeCollection-Methode. Aktualisiert den ausgewählten Wert anhand des Werts der verknüpften Zelle oder des Bereichs der Form"
type: docs
url: /de/net/aspose.cells.drawing/shapecollection/updateselectedvalue/
---
## ShapeCollection.UpdateSelectedValue method

Aktualisiert den ausgewählten Wert anhand des Werts der verknüpften Zelle oder des Bereichs des Shapes.

```csharp
public void UpdateSelectedValue()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodUpdateSelectedValueDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge der Arbeitsmappe eine Form (Dropdown-Liste) hinzu
            Aspose.Cells.Drawing.ListBox listBox = (Aspose.Cells.Drawing.ListBox)worksheet.Shapes.AddListBox(0, 0, 100, 100, 3, 20);
            
            // Lege Listenelemente und ausgewählten Wert fest
            listBox.SetInputRange("A1:A3", false, false);
            listBox.SelectedIndex = 1;
            
            // Aktualisiere den ausgewählten Wert in der Form
            worksheet.Shapes.UpdateSelectedValue();
            
            // Speichere die Arbeitsmappe
            workbook.Save("ShapeCollectionUpdateSelectedValueDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


