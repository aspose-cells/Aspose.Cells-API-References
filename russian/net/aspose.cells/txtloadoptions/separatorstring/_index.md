---
title: "TxtLoadOptions.SeparatorString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtLoadOptions. Получает и задает строковое значение в качестве разделителя"
type: docs
url: /ru/net/aspose.cells/txtloadoptions/separatorstring/
---
## TxtLoadOptions.SeparatorString property

Получает и задаёт строковое значение в качестве разделителя.

```csharp
public string SeparatorString { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertySeparatorStringDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите примерные данные с пользовательским разделителем
            worksheet.Cells["A1"].PutValue("John&Doe");
            worksheet.Cells["B1"].PutValue("30");
            worksheet.Cells["A2"].PutValue("Jane&Smith");
            worksheet.Cells["B2"].PutValue("25");

            // Сохраните с пользовательским разделителем
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.SeparatorString = "&";
            workbook.Save("output.csv", saveOptions);

            // Загрузите с тем же разделителем
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.SeparatorString = "&";
            Workbook loadedWorkbook = new Workbook("output.csv", loadOptions);

            // Проверьте загруженные данные
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];
            Console.WriteLine("A1: " + loadedSheet.Cells["A1"].StringValue);
            Console.WriteLine("B1: " + loadedSheet.Cells["B1"].StringValue);
        }
    }
}
```

### См. также

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


