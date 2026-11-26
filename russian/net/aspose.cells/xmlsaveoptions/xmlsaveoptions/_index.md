---
title: "XmlSaveOptions.XmlSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор XmlSaveOptions. Создает параметры для сохранения xml‑файла"
type: docs
url: /ru/net/aspose.cells/xmlsaveoptions/xmlsaveoptions/
---
## XmlSaveOptions constructor

Создаёт параметры для сохранения XML‑файла.

```csharp
public XmlSaveOptions()
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги с тестовыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(63);

            // Первый пример: Сохранить как XML с параметром SheetNameAsElementName
            XmlSaveOptions saveOptions1 = new XmlSaveOptions();
            saveOptions1.SheetNameAsElementName = true;
            workbook.Save("output1.xml", saveOptions1);
            
            // Второй пример: Сохранить как XML с параметрами SheetNameAsElementName и DataAsAttribute
            XmlSaveOptions saveOptions2 = new XmlSaveOptions();
            saveOptions2.SheetNameAsElementName = true;
            saveOptions2.DataAsAttribute = true;
            workbook.Save("output2.xml", saveOptions2);

            Console.WriteLine("XML files created successfully.");
        }
    }
}
```

### См. также

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


