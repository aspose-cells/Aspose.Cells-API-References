---
title: "CheckBox.CheckedValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CheckBox-egenskap. Hämtar eller anger kryssrutevärdet"
type: docs
url: /sv/net/aspose.cells.drawing/checkbox/checkedvalue/
---
## CheckBox.CheckedValue property

Hämtar eller anger kryssrutans värde.

```csharp
public CheckValueType CheckedValue { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxPropertyCheckedValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till en kryssruta i kalkylbladet
            CheckBox checkBox = sheet.Shapes.AddCheckBox(1, 1, 100, 100, 20, 20);

            // Ställ in kryssrutevärdet till Markerad
            checkBox.CheckedValue = CheckValueType.Checked;

            // Spara arbetsboken
            workbook.Save("CheckBoxCheckedValueDemo.xlsx");

            // Läs in den sparade arbetsboken för att verifiera
            Workbook loadedWorkbook = new Workbook("CheckBoxCheckedValueDemo.xlsx");
            CheckBox loadedCheckBox = (CheckBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Skriv ut kryssrutans tillstånd
            Console.WriteLine("CheckBox CheckedValue: " + loadedCheckBox.CheckedValue);
        }
    }
}
```

### Se även

* enum [CheckValueType](../../checkvaluetype/)
* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


