---
title: "ListObject.ConvertToRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ListObject. Преобразовать таблицу в диапазон"
type: docs
url: /ru/net/aspose.cells.tables/listobject/converttorange/
---
## ConvertToRange() {#converttorange}

Преобразовать таблицу в диапазон.

```csharp
public void ConvertToRange()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodConvertToRangeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("ID");
            sheet.Cells["B1"].PutValue("Name");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue("John");
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["B3"].PutValue("Mary");
            
            // Создать объект списка
            int index = sheet.ListObjects.Add("A1", "B3", true);
            ListObject listObject = sheet.ListObjects[index];
            
            Console.WriteLine("Before conversion - ListObject exists: " + (listObject != null));
            
            // Преобразовать объект списка в диапазон
            listObject.ConvertToRange();
            
            Console.WriteLine("After conversion - ListObjects count: " + sheet.ListObjects.Count);
            
            // Сохраните книгу
            workbook.Save("ListObjectConversion.xlsx");
        }
    }
}
```

### См. также

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## ConvertToRange(TableToRangeOptions) {#converttorange_1}

Преобразовать таблицу в диапазон.

```csharp
public void ConvertToRange(TableToRangeOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опции | TableToRangeOptions | опции при преобразовании таблицы в диапазон. |

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodConvertToRangeWithTableToRangeOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать примерные данные
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[0, i].PutValue($"Column {i + 1}");
                for (int row = 1; row < 5; row++)
                {
                    worksheet.Cells[row, i].PutValue(row * (i + 1));
                }
            }

            // Создайте таблицу
            int tableIndex = worksheet.ListObjects.Add(0, 0, 4, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[0].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Преобразовать таблицу в диапазон с опциями
            TableToRangeOptions options = new TableToRangeOptions();
            options.LastRow = 4;
            table.ConvertToRange(options);

            workbook.Save("TableToRangeWithOptions.xlsx");
        }
    }
}
```

### См. также

* class [TableToRangeOptions](../../tabletorangeoptions/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


