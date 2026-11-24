---
title: "IconSet.ShowValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IconSet‑Eigenschaft. Gibt an, ob die Werte der Zellen, auf die dieses Symbolset angewendet wird, angezeigt werden sollen, oder legt dies fest. Standardwert ist true"
type: docs
url: /de/net/aspose.cells/iconset/showvalue/
---
## IconSet.ShowValue property

Abrufen oder Festlegen des Flags, das angibt, ob die Werte der Zellen angezeigt werden, auf die dieses Symbolset angewendet wird. Standardwert ist true.

```csharp
public bool ShowValue { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyShowValueDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);
            sheet.Cells["A5"].PutValue(50);

            // Fügen Sie eine bedingte Formatierung für das Symbolset hinzu
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatIndex];
            int index = formatConditions.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = formatConditions[index];

            // Icon-Set-Eigenschaften festlegen
            condition.IconSet.Type = IconSetType.TrafficLights31;
            condition.IconSet.ShowValue = false; // This hides cell values and shows only icons
            condition.IconSet.Reverse = false;

            // Legen Sie den Bereich für die bedingte Formatierung fest
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 4;
            area.EndColumn = 0;
            formatConditions.AddArea(area);

            // Speichere die Arbeitsmappe
            workbook.Save("IconSetShowValueDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with icon set conditional formatting (ShowValue = false).");
        }
    }
}
```

### Siehe auch

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


