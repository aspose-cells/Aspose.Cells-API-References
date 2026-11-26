---
title: "DbfLoadOptions.DbfLoadOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор DbfLoadOptions. Параметры"
type: docs
url: /ru/net/aspose.cells.loading/dbfloadoptions/dbfloadoptions/
---
## DbfLoadOptions constructor

Параметры.

```csharp
public DbfLoadOptions()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;
    using System;

    public class DbfLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте экземпляр DbfLoadOptions, используя метод #ctor
                DbfLoadOptions loadOptions = new DbfLoadOptions();

                // Создайте книгу с параметрами загрузки DBF
                Workbook workbook = new Workbook("sample.dbf", loadOptions);

                // Получить доступ к первому листу
                Worksheet worksheet = workbook.Worksheets[0];

                // Отобразите некоторые данные из загруженного файла DBF
                Console.WriteLine("Data loaded from DBF file:");
                Console.WriteLine(worksheet.Cells["A1"].StringValue);

                // Сохраните книгу в формате Excel
                workbook.Save("DbfLoadOptionsCtorDemo.xlsx", SaveFormat.Xlsx);
                Console.WriteLine("File saved successfully with DBF data");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DbfLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [DbfLoadOptions](../)
* namespace [Aspose.Cells.Loading](../../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../../)


