---
title: "XmlLoadOptions.ConvertNumericOrDate"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство XmlLoadOptions. Указывает, преобразуется ли значение в XML‑файле в числовое или датовое"
type: docs
url: /ru/net/aspose.cells/xmlloadoptions/convertnumericordate/
---
## XmlLoadOptions.ConvertNumericOrDate property

Указывает, преобразовывать ли значение в xml‑файле в числовое или дату.

```csharp
public bool ConvertNumericOrDate { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyConvertNumericOrDateDemo
    {
        public static void Run()
        {
            // Создайте параметры загрузки XML
            XmlLoadOptions options = new XmlLoadOptions();
            
            // Установите ConvertNumericOrDate в true (по умолчанию)
            options.ConvertNumericOrDate = true;
            Workbook wb1 = new Workbook("input.xml", options);
            Cell cell1 = wb1.Worksheets[0].Cells["A1"];
            Console.WriteLine("With conversion (true): " + cell1.Value + " is type: " + cell1.Type);
            
            // Установите ConvertNumericOrDate в false
            options.ConvertNumericOrDate = false;
            Workbook wb2 = new Workbook("input.xml", options);
            Cell cell2 = wb2.Worksheets[0].Cells["A1"];
            Console.WriteLine("Without conversion (false): " + cell2.Value + " is type: " + cell2.Type);
            
            // Сохраните результаты
            wb1.Save("output_with_conversion.xlsx");
            wb2.Save("output_without_conversion.xlsx");
        }
    }
}
```

### См. также

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


