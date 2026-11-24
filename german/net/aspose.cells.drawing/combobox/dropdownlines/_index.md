---
title: "ComboBox.DropDownLines"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ComboBox Eigenschaft. Liest oder setzt die Anzahl der Listenzeilen, die im Dropdown-Bereich einer ComboBox angezeigt werden"
type: docs
url: /de/net/aspose.cells.drawing/combobox/dropdownlines/
---
## ComboBox.DropDownLines property

Liest oder setzt die Anzahl der Listenzeilen, die im Dropdown-Bereich einer ComboBox angezeigt werden.

```csharp
public int DropDownLines { get; set; }
```

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxPropertyDropDownLinesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine ComboBox mit korrekten Parametern erstellen
            ComboBox comboBox = worksheet.Shapes.AddComboBox(0, 0, 0, 0, 100, 100);
            comboBox.DropDownLines = 5;
            
            // Arbeitsblattzellen mit Elementen befüllen
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");
            worksheet.Cells["A6"].PutValue("Item 6");

            // ComboBox mit Zellwerten verknüpfen
            comboBox.InputRange = "A1:A6";

            workbook.Save("ComboBoxDropDownLinesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


