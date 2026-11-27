---
title: "ListBox.SelectedCells"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBox-egenskap. Hämtar de markerade cellerna. Returnerar null om inmatningsintervallet inte är inställt eller om ingen post är markerad"
type: docs
url: /sv/net/aspose.cells.drawing/listbox/selectedcells/
---
## ListBox.SelectedCells property

Hämtar de markerade cellerna. Returnerar null om inmatningsintervallet inte är angivet eller inget objekt är markerat.

```csharp
public Cell[] SelectedCells { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ListBoxPropertySelectedCellsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i exempeldata för ListBox-poster
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");

            // Skapa en ListBox och bind den till dataintervallet
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(7, 0, 100, 150, 5, 1);
            listBox.InputRange = "A1:A5";
            listBox.SelectionType = SelectionType.Multi;

            // Markera flera poster med nollbaserade index
            listBox.SelectedItem(0, true);
            listBox.SelectedItem(2, true);

            // Hämta och visa markerade celler
            Cell[] selectedCells = listBox.SelectedCells;
            Console.WriteLine("Selected Cells Count: " + selectedCells.Length);
            
            // Ändra markerade celler för att demonstrera åtkomst
            foreach (Cell cell in selectedCells)
            {
                Console.WriteLine("Selected Cell Address: " + cell.Name);
                cell.PutValue("[SELECTED] " + cell.StringValue);
            }

            workbook.Save("ListBoxSelectedCellsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../../../aspose.cells/cell/)
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


