---
title: "PivotField.FilterByLabel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotField. Фильтрует по заголовкам строкового или столбцового поля сводки"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/filterbylabel/
---
## PivotField.FilterByLabel method

Фильтрует по заголовкам строки или столбца сводного поля.

```csharp
public PivotFilter FilterByLabel(PivotFilterType type, string label1, string label2)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | PivotFilterType | Тип данных фильтрации. |
| label1 | String | Метка условия фильтра |
| label2 | String | Верхняя метка границы условия фильтра «между» |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterByLabelWithPivotFilterTypeStringStringDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("");
            sheet.Cells["A5"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            sheet.Cells["B5"].PutValue(40);

            // Создайте сводную таблицу с правильными параметрами
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            pivot.AddFieldToArea(PivotFieldType.Row, "Category");
            pivot.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Получить поле сводной таблицы
            PivotField field = pivot.RowFields[0];
            
            // Применить фильтры
            field.FilterByLabel(PivotFilterType.CaptionNotEqual, "(blank)", "");
            pivot.RefreshData();
            pivot.CalculateData();
            
            // Сохраните книгу
            workbook.Save("PivotFilterByLabelDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


