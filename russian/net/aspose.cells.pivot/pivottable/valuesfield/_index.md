---
title: "PivotTable.ValuesField"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Возвращает объект PivotField, представляющий все поля данных в сводной таблице. Только для чтения. Он будет создан только когда в области данных присутствует два или более поля данных. По умолчанию он находится в области строк. Вы можете перетащить его в область строк/столбцов с помощью метода PivotTable.AddFieldToArea."
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/valuesfield/
---
## PivotTable.ValuesField property

Возвращает объект [`PivotField`](../../pivotfield/), представляющий все поля данных в сводной таблице. Только для чтения. Он будет создан только когда в области данных присутствует два или более полей данных. По умолчанию он находится в области строк. Вы можете перетащить его в область строк/столбцов с помощью метода PivotTable.AddFieldToArea() .

```csharp
public PivotField ValuesField { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyValuesFieldDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(1500);
            worksheet.Cells["A4"].PutValue("Product A");
            worksheet.Cells["B4"].PutValue("South");
            worksheet.Cells["C4"].PutValue(2000);
            worksheet.Cells["A5"].PutValue("Product B");
            worksheet.Cells["B5"].PutValue("North");
            worksheet.Cells["C5"].PutValue(1200);

            try
            {
                // Создайте сводную таблицу
                int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Добавить поля в области
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

                // Вычислить данные для заполнения сводной таблицы
                pivotTable.CalculateData();

                // Получите доступ к свойству ValuesField (только для чтения)
                PivotField valuesField = pivotTable.ValuesField;

                if (valuesField != null)
                {
                    Console.WriteLine("ValuesField Name: " + valuesField.Name);
                    Console.WriteLine("ValuesField DisplayName: " + valuesField.DisplayName);
                    Console.WriteLine("ValuesField Position: " + valuesField.Position);
                    Console.WriteLine("ValuesField RegionType: " + valuesField.RegionType);
                    Console.WriteLine("ValuesField IsValuesField: " + valuesField.IsValuesField);
                }
                else
                {
                    Console.WriteLine("ValuesField is null - no data fields in the pivot table");
                }

                // Сохраните книгу
                workbook.Save("PivotTableValuesFieldDemo.xlsx");
                Console.WriteLine("PivotTable with ValuesField demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


