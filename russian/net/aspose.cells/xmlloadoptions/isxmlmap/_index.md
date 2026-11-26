---
title: "XmlLoadOptions.IsXmlMap"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство XmlLoadOptions. Указывает, выполняется ли сопоставление XML с Excel. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/xmlloadoptions/isxmlmap/
---
## XmlLoadOptions.IsXmlMap property

Указывает, следует ли сопоставлять XML с Excel. Значение по умолчанию — false.

```csharp
public bool IsXmlMap { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyIsXmlMapDemo
    {
        public static void Run()
        {
            // Создайте экземпляр XmlLoadOptions
            XmlLoadOptions options = new XmlLoadOptions();

            // Включите сопоставление XML при загрузке файла
            options.IsXmlMap = true;

            // Загрузите XML‑файл в Workbook, используя указанные параметры
            Workbook workbook = new Workbook("sample.xml", options);

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Отобразите некоторые данные из загруженного XML, чтобы продемонстрировать успешное сопоставление
            Console.WriteLine("Data from loaded XML:");
            Console.WriteLine(worksheet.Cells["A1"].StringValue);
            Console.WriteLine(worksheet.Cells["A2"].StringValue);

            // Сохраните книгу в новый файл Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


