---
title: "ComboBox.DropDownLines"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ComboBox‑egenskap. Hämtar eller anger antalet listlinjer som visas i kombinationsrutans rullgardinsdel"
type: docs
url: /sv/net/aspose.cells.drawing/combobox/dropdownlines/
---
## ComboBox.DropDownLines property

Hämtar eller anger antalet listrader som visas i rullgardinsdelen av en kombinationsruta.

```csharp
public int DropDownLines { get; set; }
```

### Exempel

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

            // Skapa en ComboBox med korrekta parametrar
            ComboBox comboBox = worksheet.Shapes.AddComboBox(0, 0, 0, 0, 100, 100);
            comboBox.DropDownLines = 5;
            
            // Fyll kalkylbladsceller med objekt
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");
            worksheet.Cells["A6"].PutValue("Item 6");

            // Länka kombinationsrutan till cellvärden
            comboBox.InputRange = "A1:A6";

            workbook.Save("ComboBoxDropDownLinesDemo.xlsx");
        }
    }
}
```

### Se även

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


