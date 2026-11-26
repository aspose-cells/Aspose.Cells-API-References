---
title: "Перечисление PivotAreaType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Pivot.PivotAreaType. Указывает тип правила, используемого для описания области или аспекта сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotareatype/
---
## PivotAreaType enumeration

Указывает тип правила, используемого для описания области или аспекта PivotTable.

```csharp
public enum PivotAreaType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Нет области Pivot. |
| Normal | `1` | Представляет заголовок или элемент. |
| Data | `2` | Представляет объект в области данных. |
| All | `3` | Представляет всю сводную таблицу. |
| Origin | `4` | Представляет пустые ячейки в левом верхнем углу сводной таблицы (в правом верхнем для листов RTL). |
| Button | `5` | Представляет кнопку поля. |
| TopRight | `6` | Представляет пустые ячейки в правом верхнем углу сводной таблицы (в левом верхнем для листов RTL). |

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotAreaTypeDemo
    {
        public static void PivotAreaTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apples");
            worksheet.Cells["A3"].PutValue("Oranges");
            worksheet.Cells["A4"].PutValue("Bananas");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);

            // Создать сводную таблицу
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // Создать PivotArea для сводной таблицы
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.OnlyData = true;
            pivotArea.IsRowGrandIncluded = true;

            // Вывести свойства PivotArea
            Console.WriteLine("Pivot Area Type: " + pivotArea.RuleType);
            Console.WriteLine("Only Data: " + pivotArea.OnlyData);
            Console.WriteLine("Is Row Grand Included: " + pivotArea.IsRowGrandIncluded);

            // Сохраните книгу
            workbook.Save("PivotAreaTypeExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


