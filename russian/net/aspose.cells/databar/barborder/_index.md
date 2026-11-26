---
title: "DataBar.BarBorder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataBar. Возвращает объект, который определяет границу полосы данных"
type: docs
url: /ru/net/aspose.cells/databar/barborder/
---
## DataBar.BarBorder property

Получает объект, определяющий границу полосы данных.

```csharp
public DataBarBorder BarBorder { get; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyBarBorderDemo
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
            int conditionIdx = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIdx];

            // Установить свойства полосы данных
            fc.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            fc.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            fc.DataBar.Color = Color.Blue;
            fc.DataBar.ShowValue = true;

            // Установить свойства границы столбца
            fc.DataBar.BarBorder.Type = DataBarBorderType.Solid;
            fc.DataBar.BarBorder.Color = Color.Black;

            // Сохраните книгу
            workbook.Save("DataBarBorderDemo.xlsx");
        }
    }
}
```

### См. также

* class [DataBarBorder](../../databarborder/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


