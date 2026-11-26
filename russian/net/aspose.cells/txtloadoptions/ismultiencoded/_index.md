---
title: "TxtLoadOptions.IsMultiEncoded"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtLoadOptions. True означает, что файл содержит несколько кодировок"
type: docs
url: /ru/net/aspose.cells/txtloadoptions/ismultiencoded/
---
## TxtLoadOptions.IsMultiEncoded property

True означает, что файл содержит несколько кодировок.

```csharp
public bool IsMultiEncoded { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyIsMultiEncodedDemo
    {
        public static void Run()
        {
            // Создайте параметры загрузки текста
            TxtLoadOptions options = new TxtLoadOptions();
            
            // Установите IsMultiEncoded в true, чтобы обрабатывать несколько кодировок
            options.IsMultiEncoded = true;
            
            // Загрузите книгу с параметрами
            Workbook workbook = new Workbook("example.csv", options);
            
            // Отобразите примерные значения из загруженного файла
            Console.WriteLine("A2 Cell Value: " + workbook.Worksheets[0].Cells["A2"].StringValue);
            Console.WriteLine("A3 Cell Value: " + workbook.Worksheets[0].Cells["A3"].StringValue);
        }
    }
}
```

### См. также

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


