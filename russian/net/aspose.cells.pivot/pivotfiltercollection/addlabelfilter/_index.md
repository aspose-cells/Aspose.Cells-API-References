---
title: "PivotFilterCollection.AddLabelFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotFilterCollection. Фильтрует по подписям строкового или столбцового PivotField"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfiltercollection/addlabelfilter/
---
## PivotFilterCollection.AddLabelFilter method

Фильтрует по заголовкам строки или столбца сводного поля.

```csharp
public PivotFilter AddLabelFilter(int baseFieldIndex, PivotFilterType type, string label1, 
    string label2)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| baseFieldIndex | Int32 | Индекс поля в источнике. |
| type | PivotFilterType | Тип данных фильтрации. |
| label1 | String | Метка условия фильтра |
| label2 | String | Верхняя метка границы условия фильтра «между» |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodAddLabelFilterWithInt32PivotFilterTypeStringStriDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Cherry";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                PivotFilterCollection filters = pivotTable.PivotFilters;
                
                // Добавить фильтр метки, чтобы показывать товары, начинающиеся с "A"
                PivotFilter filter = filters.AddLabelFilter(
                    baseFieldIndex: 0,
                    type: PivotFilterType.CaptionBeginsWith,
                    label1: "A",
                    label2: null
                );

                Console.WriteLine($"Label filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, Value1: {filter.Value1}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding label filter: {ex.Message}");
            }
            
            workbook.Save("PivotFilterCollectionMethodAddLabelFilterDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


