---
title: "DataBar.MaxLength"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataBar. Представляет максимальную длину полосы данных"
type: docs
url: /ru/net/aspose.cells/databar/maxlength/
---
## DataBar.MaxLength property

Представляет максимальную длину data bar.

```csharp
public int MaxLength { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMaxLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Добавить условное форматирование
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[formatIndex];
            
            CellArea area = new CellArea
            {
                StartRow = 0,
                EndRow = 3,
                StartColumn = 0,
                EndColumn = 0
            };
            fcc.AddArea(area);

            // Добавить полосу данных и установить свойства
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            DataBar dataBar = fcc[conditionIndex].DataBar;
            
            dataBar.Color = Color.Blue;
            dataBar.MinLength = 0;
            dataBar.MaxLength = 90; // Demonstrating MaxLength property
            
            workbook.Save("DataBarMaxLengthDemo.xlsx");
        }
    }
}
```

### См. также

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


