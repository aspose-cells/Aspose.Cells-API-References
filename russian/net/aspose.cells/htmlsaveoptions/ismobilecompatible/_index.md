---
title: "HtmlSaveOptions.IsMobileCompatible"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, совместим ли выводимый HTML с мобильными устройствами. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/ismobilecompatible/
---
## HtmlSaveOptions.IsMobileCompatible property

Указывает, совместим ли выводимый HTML с мобильными устройствами. Значение по умолчанию — false.

```csharp
public bool IsMobileCompatible { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsMobileCompatibleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Mobile Compatibility Test");

            // Создать параметры сохранения HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Установите совместимость с мобильными устройствами
            saveOptions.IsMobileCompatible = true;

            // Сохраните с включённой совместимостью с мобильными устройствами
            workbook.Save("MobileCompatible.html", saveOptions);

            // Измените на несовместимый с мобильными устройствами
            saveOptions.IsMobileCompatible = false;
            workbook.Save("NonMobileCompatible.html", saveOptions);
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


