---
title: "PivotAreaFilterCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotAreaFilterCollection. Возвращает фильтр из списка по индексу."
type: docs
url: /ru/net/aspose.cells.pivot/pivotareafiltercollection/item/
---
## PivotAreaFilterCollection indexer

Получает фильтр из списка по индексу.

```csharp
public PivotAreaFilter this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaFilterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            
            // Добавьте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Добавить поля в области сводной таблицы
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Создать условное форматирование
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[pivotTable.ConditionalFormats.Add()];
            pcf.ScopeType = PivotConditionFormatScopeType.Field;
            
            // Создайте область сводной таблицы и добавьте фильтры
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Data, "Value");
            pcf.PivotAreas.Add(pivotArea);
            
            // Продемонстрировать использование свойства Item
            PivotAreaFilter filter = pivotArea.Filters[0];
            filter.IsSubtotalSet(PivotFieldSubtotalType.Automatic);
            
            // Сохраните книгу
            workbook.Save("PivotAreaFilterCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotAreaFilter](../../pivotareafilter/)
* class [PivotAreaFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


