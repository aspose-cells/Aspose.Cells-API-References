---
title: "HtmlSaveOptions.IsFullPathLink"
second_title: "Справочник API Aspose.Cells для .NET"
description: "HtmlSaveOptions property. Указывает, используется ли полная ссылка пути в sheet00x.htmfilelist.xml и tabstrip.htm. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/isfullpathlink/
---
## HtmlSaveOptions.IsFullPathLink property

Указывает, использовать ли полные пути в ссылках в файлах sheet00x.htm, filelist.xml и tabstrip.htm. Значение по умолчанию — false.

```csharp
public bool IsFullPathLink { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsFullPathLinkDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test HTML Export");

            // Создать параметры сохранения HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Продемонстрировать свойство IsFullPathLink
            saveOptions.IsFullPathLink = true; // Set to true to use full path links
            
            // Сохранить с различными настройками IsFullPathLink
            workbook.Save("HtmlExport_FullPathLinks.html", saveOptions);
            
            saveOptions.IsFullPathLink = false; // Set to false for relative paths
            workbook.Save("HtmlExport_RelativeLinks.html", saveOptions);
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


