---
title: "XmlSaveOptions.DataAsAttribute"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство XmlSaveOptions. Указывает, экспортируются ли данные как атрибуты элемента"
type: docs
url: /ru/net/aspose.cells/xmlsaveoptions/dataasattribute/
---
## XmlSaveOptions.DataAsAttribute property

Указывает, экспортировать ли данные как атрибуты элемента.

```csharp
public bool DataAsAttribute { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyDataAsAttributeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Создайте параметры сохранения XML с DataAsAttribute, установленным в true
            XmlSaveOptions saveOptions = new XmlSaveOptions
            {
                DataAsAttribute = true,
                SheetNameAsElementName = true
            };

            // Сохранить данные как атрибуты
            workbook.Save("DataAsAttribute_True.xml", saveOptions);

            // Изменить, чтобы сохранять данные как элементы
            saveOptions.DataAsAttribute = false;
            workbook.Save("DataAsAttribute_False.xml", saveOptions);
        }
    }
}
```

### См. также

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


