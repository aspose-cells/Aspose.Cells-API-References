---
title: "HtmlSaveOptions.IsIECompatible"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, совместим ли выводимый HTML с браузером IE. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/isiecompatible/
---
## HtmlSaveOptions.IsIECompatible property

Указывает, совместим ли выводимый HTML с браузером IE. Значение по умолчанию — false.

```csharp
public bool IsIECompatible { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsIECompatibleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("HTML Export Demo");

            // Создать параметры сохранения HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Установить свойство IsIECompatible
            saveOptions.IsIECompatible = false; // Disable IE compatibility mode
            
            // Сохранить рабочую книгу с параметрами HTML
            workbook.Save("HtmlExportDemo.html", saveOptions);

            Console.WriteLine("HTML file saved with IsIECompatible = false");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


