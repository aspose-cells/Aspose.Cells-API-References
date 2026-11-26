---
title: "LoadOptions.IgnoreNotPrinted"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Игнорировать данные, которые не печатаются при прямой печати файла"
type: docs
url: /ru/net/aspose.cells/loadoptions/ignorenotprinted/
---
## LoadOptions.IgnoreNotPrinted property

Игнорировать данные, которые не печатаются при прямой печати файла

```csharp
public bool IgnoreNotPrinted { get; set; }
```

### Примечания

Только для файла xlsx.

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyIgnoreNotPrintedDemo
    {
        public static void Run()
        {
            // Создайте параметры загрузки HTML и установите IgnoreNotPrinted
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.AutoFitColsAndRows = true;

            // Загрузить HTML‑файл с указанными параметрами
            Workbook workbook = new Workbook("example.html", loadOptions);
            Worksheet worksheet = workbook.Worksheets[0];

            // Продемонстрируйте эффект IgnoreNotPrinted, проверяя стили ячеек
            Console.WriteLine("B3 Cell Color: " + worksheet.Cells["B3"].GetStyle().ForegroundColor);
            Console.WriteLine("B4 Cell Color: " + worksheet.Cells["B4"].GetStyle().ForegroundColor);
            Console.WriteLine("B5 Cell Color: " + worksheet.Cells["B5"].GetStyle().ForegroundColor);

            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


