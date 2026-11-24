---
title: "ComboBox.SelectedValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ComboBox Eigenschaft. Gibt den ausgewählten Wert der ComboBox zurück"
type: docs
url: /de/net/aspose.cells.drawing/combobox/selectedvalue/
---
## ComboBox.SelectedValue property

Liest den ausgewählten Wert der ComboBox.

```csharp
public string SelectedValue { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxPropertySelectedValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle ein ComboBox und füge Elemente hinzu
            Aspose.Cells.Drawing.ComboBox comboBox = (Aspose.Cells.Drawing.ComboBox)worksheet.Shapes.AddComboBox(1, 0, 1, 0, 100, 50);
            comboBox.LinkedCell = "A1";
            comboBox.SetInputRange("B1:B4", false, false);
            
            // Setze Werte im Eingabebereich
            worksheet.Cells["B1"].PutValue("a");
            worksheet.Cells["B2"].PutValue("b");
            worksheet.Cells["B3"].PutValue("c");
            worksheet.Cells["B4"].PutValue("d");

            // Demonstriere SelectedValue (schreibgeschützte Eigenschaft)
            Console.WriteLine("SelectedValue: " + comboBox.SelectedValue);

            // Speichere die Arbeitsmappe
            workbook.Save("ComboBoxDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


