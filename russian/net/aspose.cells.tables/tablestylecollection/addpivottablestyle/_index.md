---
title: "TableStyleCollection.AddPivotTableStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод TableStyleCollection. Добавляет пользовательский стиль сводной таблицы"
type: docs
url: /ru/net/aspose.cells.tables/tablestylecollection/addpivottablestyle/
---
## TableStyleCollection.AddPivotTableStyle method

Добавляет пользовательский стиль сводной таблицы.

```csharp
public int AddPivotTableStyle(string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя стиля сводной таблицы. |

### Возвращаемое значение

Индекс стиля сводной таблицы.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleCollectionMethodAddPivotTableStyleWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Desktop");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(800);
            worksheet.Cells["A4"].PutValue("Tablet");
            worksheet.Cells["B4"].PutValue("East");
            worksheet.Cells["C4"].PutValue(500);

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, 1);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 2);

            try
            {
                // Получить коллекцию стилей таблицы
                TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

                // Вызвать AddPivotTableStyle с параметром типа String
                int styleIndex = tableStyles.AddPivotTableStyle("CustomPivotStyle1");
                Console.WriteLine($"Added pivot table style at index: {styleIndex}");

                // Установить новый стиль в качестве стиля сводной таблицы по умолчанию
                tableStyles.DefaultPivotStyleName = "CustomPivotStyle1";

                // Применить стиль к нашей сводной таблице
                pivotTable.PivotTableStyleName = "CustomPivotStyle1";
                Console.WriteLine("Applied custom pivot table style successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddPivotTableStyle method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("TableStyleCollectionMethodAddPivotTableStyleWithStringDemo.xlsx");
        }
    }
}
```

### См. также

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


