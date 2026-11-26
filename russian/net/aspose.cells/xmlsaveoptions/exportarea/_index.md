---
title: "XmlSaveOptions.ExportArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство XmlSaveOptions. Получает или задает диапазон экспорта"
type: docs
url: /ru/net/aspose.cells/xmlsaveoptions/exportarea/
---
## XmlSaveOptions.ExportArea property

Получает или задает диапазон экспорта.

```csharp
public CellArea ExportArea { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните данные в листе
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Создайте XmlSaveOptions и установите ExportArea
            XmlSaveOptions saveOptions = new XmlSaveOptions
            {
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 }
            };

            // Сохранить только указанную область в XML
            workbook.Save("ExportAreaDemo.xml", saveOptions);
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


