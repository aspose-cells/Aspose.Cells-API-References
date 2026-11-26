---
title: "Перечисление PivotLineType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Pivot.PivotLineType. Указывает тип PivotLine"
type: docs
url: /ru/net/aspose.cells.pivot/pivotlinetype/
---
## PivotLineType enumeration

Указывает тип PivotLine.

```csharp
public enum PivotLineType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Regular | `0` | Обычная PivotLine с элементами pivot. |
| Subtotal | `1` | Строка подытога. |
| GrandTotal | `2` | Строка общего итога. |
| Blank | `3` | Пустая строка после каждой группы. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotLineTypeDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Создать сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Добавить поле строки и поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Сортировать поле строки по значениям в порядке убывания
            pivotTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "B2");
            
            // Вычислить данные сводной таблицы
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("PivotLineTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


