---
title: "TxtSaveOptions.Encoding"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtSaveOptions. Получает и задает кодировку по умолчанию"
type: docs
url: /ru/net/aspose.cells/txtsaveoptions/encoding/
---
## TxtSaveOptions.Encoding property

Получает и задает кодировку по умолчанию.

```csharp
public Encoding Encoding { get; set; }
```

### Примеры

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyEncodingDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            
            // Создайте параметры сохранения TXT с кодировкой ASCII
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                Separator = '\t'
            };
            
            // Сохраните книгу с указанной кодировкой
            workbook.Save("output.txt", saveOptions);
            
            Console.WriteLine("File saved with ASCII encoding");
        }
    }
}
```

### См. также

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


