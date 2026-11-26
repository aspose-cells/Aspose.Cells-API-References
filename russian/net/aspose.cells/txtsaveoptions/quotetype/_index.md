---
title: "TxtSaveOptions.QuoteType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtSaveOptions. Получает или задает способ заключения значений в кавычки в экспортируемом текстовом файле"
type: docs
url: /ru/net/aspose.cells/txtsaveoptions/quotetype/
---
## TxtSaveOptions.QuoteType property

Получает или задает, как заключать значения в кавычки в экспортируемом текстовом файле.

```csharp
public TxtValueQuoteType QuoteType { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyQuoteTypeDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги с тестовыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Text");
            worksheet.Cells["B1"].PutValue("123");
            worksheet.Cells["A2"].PutValue("Another text");
            worksheet.Cells["B2"].PutValue("=1+2");

            // Сохраните с QuoteType.Normal (по умолчанию)
            MemoryStream stream1 = new MemoryStream();
            workbook.Save(stream1, new TxtSaveOptions()
            {
                Encoding = Encoding.ASCII
            });
            
            // Сохраните с QuoteType.Always
            MemoryStream stream2 = new MemoryStream();
            workbook.Save(stream2, new TxtSaveOptions()
            {
                Encoding = Encoding.ASCII,
                QuoteType = TxtValueQuoteType.Always
            });

            // Отобразить пример вывода
            Console.WriteLine("Normal QuoteType:");
            Console.WriteLine(Encoding.ASCII.GetString(stream1.ToArray()));
            
            Console.WriteLine("\nAlways QuoteType:");
            Console.WriteLine(Encoding.ASCII.GetString(stream2.ToArray()));
        }
    }
}
```

### См. также

* enum [TxtValueQuoteType](../../txtvaluequotetype/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


