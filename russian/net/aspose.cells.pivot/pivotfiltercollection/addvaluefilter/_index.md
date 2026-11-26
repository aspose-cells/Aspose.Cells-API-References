---
title: "PivotFilterCollection.AddValueFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotFilterCollection. Фильтрует по значениям поля сводных данных"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfiltercollection/addvaluefilter/
---
## PivotFilterCollection.AddValueFilter method

Фильтрует по значениям данных сводного поля.

```csharp
public PivotFilter AddValueFilter(int baseFieldIndex, int valueFieldIndex, PivotFilterType type, 
    double value1, double value2)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| baseFieldIndex | Int32 | Индекс поля в источнике. |
| valueFieldIndex | Int32 | Индекс поля значения в области значений. |
| type | PivotFilterType | Тип данных фильтрации. |
| value1 | Double | Значение условия фильтра |
| value2 | Double | Верхнее значение условия фильтра «между» |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFilterCollectionMethodAddValueFilterWithInt32Int32PivotFilterTypeDoublDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Widget";
            worksheet.Cells["A3"].Value = "Gadget";
            worksheet.Cells["A4"].Value = "Thingy";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["B2"].Value = 15.99;
            worksheet.Cells["B3"].Value = 24.99;
            worksheet.Cells["B4"].Value = 9.99;

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
                
                // Добавить фильтр значений, чтобы показывать товары с ценой от $10 до $20
                PivotFilter filter = filters.AddValueFilter(
                    baseFieldIndex: 0,
                    valueFieldIndex: 1,
                    type: PivotFilterType.ValueBetween,
                    value1: 10.0,
                    value2: 20.0
                );

                Console.WriteLine($"Value filter added successfully. Filter type: {filter.FilterType}");
                Console.WriteLine($"Field index: {filter.FieldIndex}, Value field index: {filter.ValueFieldIndex}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding value filter: {ex.Message}");
            }
            
            workbook.Save("PivotFilterCollectionMethodAddValueFilterDemo.xlsx");
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


