---
title: "DataBar.AxisPosition"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataBar. Получает или задает положение оси гистограмм, указанной правилом условного форматирования"
type: docs
url: /ru/net/aspose.cells/databar/axisposition/
---
## DataBar.AxisPosition property

Получает или задает положение оси полос данных, указанное правилом условного форматирования.

```csharp
public DataBarAxisPosition AxisPosition { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyAxisPositionDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["E3"].PutValue(10);
            sheet.Cells["E4"].PutValue(20);
            sheet.Cells["F3"].PutValue(30);
            sheet.Cells["F4"].PutValue(40);
            sheet.Cells["G3"].PutValue(-15);
            sheet.Cells["G4"].PutValue(-25);

            // Добавить условное форматирование полос данных
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection conds = sheet.ConditionalFormattings[formatIndex];
            int idx = conds.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = conds[idx];
            
            // Настроить свойства гистограммы
            cond.DataBar.Color = Color.Orange;
            cond.DataBar.MinCfvo.Type = FormatConditionValueType.AutomaticMin;
            cond.DataBar.MaxCfvo.Type = FormatConditionValueType.AutomaticMax;
            cond.DataBar.ShowValue = false;
            
            // Установить положение оси (основная демонстрация)
            cond.DataBar.AxisPosition = DataBarAxisPosition.Automatic;
            cond.DataBar.AxisColor = Color.Red;

            // Сохраните книгу
            workbook.Save("DataBarAxisPositionDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("DataBar with AxisPosition demo created successfully.");
        }
    }
}
```

### См. также

* enum [DataBarAxisPosition](../../databaraxisposition/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


