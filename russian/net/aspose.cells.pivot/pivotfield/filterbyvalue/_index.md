---
title: "PivotField.FilterByValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotField. Фильтрует по значениям данных сводного поля"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/filterbyvalue/
---
## PivotField.FilterByValue method

Фильтрует по значениям данных сводного поля.

```csharp
public PivotFilter FilterByValue(int valueFieldIndex, PivotFilterType type, double value1, 
    double value2)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
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

    public class PivotFieldMethodFilterByValueWithInt32PivotFilterTypeDoubleDoubDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["B2"].Value = 2.5;
            worksheet.Cells["B3"].Value = 1.8;
            worksheet.Cells["B4"].Value = 3.2;
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["C2"].Value = 100;
            worksheet.Cells["C3"].Value = 150;
            worksheet.Cells["C4"].Value = 80;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Добавить поля данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Получить поле сводной таблицы
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Вызовите метод FilterByValue с параметрами (Int32, PivotFilterType, Double, Double)
                // Отфильтруйте продукты, у которых Quantity (индекс поля 1) находится между 90 и 160
                PivotFilter filter = pivotField.FilterByValue(1, PivotFilterType.ValueBetween, 90.0, 160.0);

                Console.WriteLine("FilterByValue method executed successfully");
                Console.WriteLine($"Filter type: {filter.FilterType}");
                Console.WriteLine($"Value field index: {filter.ValueFieldIndex}");

                // Обновите сводную таблицу, чтобы отобразить изменения
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FilterByValue method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("PivotFieldMethodFilterByValueDemo.xlsx");
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


