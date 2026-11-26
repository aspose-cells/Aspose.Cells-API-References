---
title: "PivotPageFields.PageFieldCount"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotPageFields. Возвращает количество полей страницы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotpagefields/pagefieldcount/
---
## PivotPageFields.PageFieldCount property

Получает количество полей страниц.

```csharp
public int PageFieldCount { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotPageFieldsPropertyPageFieldCountDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Создайте образцы листов с данными
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "Data1";
            FillSampleData(sheet1);

            Worksheet sheet2 = workbook.Worksheets.Add("Data2");
            FillSampleData(sheet2);

            // Создайте лист сводной таблицы
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");

            // Создайте экземпляр PivotPageFields
            PivotPageFields pageFields = new PivotPageFields();

            // Добавьте поля страницы, чтобы продемонстрировать свойство PageFieldCount
            pageFields.AddPageField(new string[] { "Category1", "Category2" });
            pageFields.AddPageField(new string[] { "Region1", "Region2" });

            try
            {
                // Отобразите значение свойства PageFieldCount
                Console.WriteLine("Number of page fields: " + pageFields.PageFieldCount);

                // Добавьте идентификацию для полей страницы
                pageFields.AddIdentify(0, new int[] { 0, 1 });
                pageFields.AddIdentify(1, new int[] { 1, 0 });

                // Проверьте, что количество осталось прежним после добавления идентификаций
                Console.WriteLine("PageFieldCount after adding identifications: " + pageFields.PageFieldCount);

                // Создайте сводную таблицу, используя поля страницы
                string[] sources = { "=Data1!A1:C4", "=Data2!A1:C4" };
                pivotSheet.PivotTables.Add(sources, false, pageFields, "E3", "DemoPivot");

                // Сохраните книгу
                workbook.Save("PageFieldCountDemo.xlsx");
                Console.WriteLine("Demo completed successfully. File saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private static void FillSampleData(Worksheet sheet)
        {
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Value");

            cells["A2"].PutValue("Category1");
            cells["B2"].PutValue("Region1");
            cells["C2"].PutValue(100);

            cells["A3"].PutValue("Category2");
            cells["B3"].PutValue("Region2");
            cells["C3"].PutValue(200);
        }
    }
}
```

### См. также

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


