---
title: "LoadFilter.LoadDataFilterOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadFilter. Параметры фильтра, указывающие, какие данные следует загружать"
type: docs
url: /ru/net/aspose.cells/loadfilter/loaddatafilteroptions/
---
## LoadFilter.LoadDataFilterOptions property

Параметры фильтра, указывающие, какие данные следует загрузить.

```csharp
public LoadDataFilterOptions LoadDataFilterOptions { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterPropertyLoadDataFilterOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = 123;
            worksheet.Cells["C1"].Formula = "=SUM(A1:B1)";

            try
            {
                // Создать экземпляр LoadFilter с опциями по умолчанию
                LoadFilter loadFilter = new LoadFilter();

                // Отобразить значение LoadDataFilterOptions по умолчанию
                Console.WriteLine("Default LoadDataFilterOptions: " + loadFilter.LoadDataFilterOptions);

                // Установить новые параметры фильтра (комбинация флагов)
                loadFilter.LoadDataFilterOptions = LoadDataFilterOptions.CellValue | LoadDataFilterOptions.Formula;

                // Отобразить обновлённое значение
                Console.WriteLine("Updated LoadDataFilterOptions: " + loadFilter.LoadDataFilterOptions);

                // Создать другой фильтр с другими параметрами
                LoadFilter anotherFilter = new LoadFilter(LoadDataFilterOptions.Chart | LoadDataFilterOptions.Picture);

                // Отобразить параметры из конструктора
                Console.WriteLine("Constructor LoadDataFilterOptions: " + anotherFilter.LoadDataFilterOptions);

                // Сохраните книгу
                workbook.Save("LoadDataFilterOptionsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* enum [LoadDataFilterOptions](../../loaddatafilteroptions/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


