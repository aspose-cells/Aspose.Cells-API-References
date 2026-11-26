---
title: "DifLoadOptions.DifLoadOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор DifLoadOptions. Параметры"
type: docs
url: /ru/net/aspose.cells.loading/difloadoptions/difloadoptions/
---
## DifLoadOptions constructor

Параметры.

```csharp
public DifLoadOptions()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;
    using System;

    public class DifLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новый экземпляр DifLoadOptions, используя конструктор без параметров
                DifLoadOptions loadOptions = new DifLoadOptions();

                // Создать новую книгу с параметрами по умолчанию
                Workbook workbook = new Workbook();

                // Получить доступ к первому листу
                Worksheet worksheet = workbook.Worksheets[0];

                // Добавить примерные данные, чтобы продемонстрировать работоспособность книги
                worksheet.Cells["A1"].PutValue("DifLoadOptions Constructor Demo");
                worksheet.Cells["A2"].PutValue("Created at: " + DateTime.Now.ToString());
                worksheet.Cells["A4"].PutValue("This demonstrates using the parameterless constructor");

                // Сохраните книгу в формате DIF
                workbook.Save("DifLoadOptionsCtorDemo.dif", SaveFormat.Dif);

                // Теперь загрузите сохранённый файл DIF с помощью DifLoadOptions
                DifLoadOptions difOptions = new DifLoadOptions();
                Workbook loadedWorkbook = new Workbook("DifLoadOptionsCtorDemo.dif", difOptions);

                // Сохраните загруженные данные в XLSX для проверки
                loadedWorkbook.Save("DifLoadOptionsCtorVerification.xlsx", SaveFormat.Xlsx);

                Console.WriteLine("DifLoadOptions constructor demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DifLoadOptions constructor demo: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [DifLoadOptions](../)
* namespace [Aspose.Cells.Loading](../../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../../)


