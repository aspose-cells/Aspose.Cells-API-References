---
title: "TxtSaveOptions.AlwaysQuoted"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtSaveOptions. Указывает, следует ли всегда добавлять '\"' для каждого поля. Если true, то все значения будут заключены в кавычки. Если false, то значения будут заключены в кавычки только при необходимости (например, когда значения содержат специальные символы, такие как '\"', '\\\\n' или разделительный символ). По умолчанию false."
type: docs
url: /ru/net/aspose.cells/txtsaveoptions/alwaysquoted/
---
## TxtSaveOptions.AlwaysQuoted property

Указывает, следует ли всегда добавлять '"' для каждого поля. Если true, то все значения будут заключены в кавычки; если false, то значения будут заключены в кавычки только при необходимости (например, когда значения содержат специальные символы, такие как '"', '\\n' или разделительный символ). По умолчанию false.

```csharp
[Obsolete("Use QuoteType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AlwaysQuoted { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство QuoteType. Это свойство будет удалено через 12 месяцев, начиная с августа 2012 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyAlwaysQuotedDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200.50);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(899.99);

            // Создайте TxtSaveOptions с AlwaysQuoted, установленным в true
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Separator = ',',
                AlwaysQuoted = true,
                QuoteType = TxtValueQuoteType.Always
            };

            // Сохраните с кавычками вокруг всех значений
            workbook.Save("AlwaysQuoted_True.txt", saveOptions);

            // Измените на false и сохраните снова
            saveOptions.AlwaysQuoted = false;
            workbook.Save("AlwaysQuoted_False.txt", saveOptions);

            Console.WriteLine("Files saved with different AlwaysQuoted settings.");
        }
    }
}
```

### См. также

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


