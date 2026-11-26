---
title: "OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OdsLoadOptions. Указывает, применяется ли стиль Excel по умолчанию к гиперссылке"
type: docs
url: /ru/net/aspose.cells/odsloadoptions/applyexceldefaultstyletohyperlink/
---
## OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink property

Указывает, применяется ли стиль Excel по умолчанию к гиперссылке.

```csharp
public bool ApplyExcelDefaultStyleToHyperlink { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsLoadOptionsPropertyApplyExcelDefaultStyleToHyperlinkDemo
    {
        public static void Run()
        {
            // Создайте экземпляр OdsLoadOptions
            OdsLoadOptions loadOptions = new OdsLoadOptions();

            // Установить свойство ApplyExcelDefaultStyleToHyperlink
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;

            // Загрузите файл ODS с указанными параметрами
            Workbook workbook = new Workbook("sample.ods", loadOptions);

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить гиперссылку для демонстрации применения стиля
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // Сохраните книгу в новый файл
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


