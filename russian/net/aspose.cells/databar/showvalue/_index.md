---
title: "DataBar.ShowValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataBar. Получить или установить флаг, указывающий, показывать ли значения ячеек, к которым применена эта гистограмма. Значение по умолчанию — true"
type: docs
url: /ru/net/aspose.cells/databar/showvalue/
---
## DataBar.ShowValue property

Получить или установить флаг, указывающий, показывать ли значения ячеек, к которым применён этот data bar. Значение по умолчанию — true.

```csharp
public bool ShowValue { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyShowValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Добавить условное форматирование полос данных
            int idx = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Добавить условие гистограммы
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];
            
            // Установить свойства полосы данных
            fc.DataBar.MinCfvo.Type = FormatConditionValueType.Min;
            fc.DataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.DataBar.Color = Color.Green;
            
            // Продемонстрировать свойство ShowValue
            fc.DataBar.ShowValue = true; // Show cell values along with data bars
            
            // Сохраните книгу
            workbook.Save("DataBarShowValueDemo.xlsx");
            
            Console.WriteLine("DataBar ShowValue demo completed. Output file: DataBarShowValueDemo.xlsx");
        }
    }
}
```

### См. также

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


