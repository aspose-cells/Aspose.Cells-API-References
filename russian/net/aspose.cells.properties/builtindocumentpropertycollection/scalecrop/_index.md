---
title: "BuiltInDocumentPropertyCollection.ScaleCrop"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Указывает режим отображения миниатюры документа"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/scalecrop/
---
## BuiltInDocumentPropertyCollection.ScaleCrop property

Указывает режим отображения миниатюры документа.

```csharp
public bool ScaleCrop { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyScaleCropDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к встроенным свойствам документа
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Установить свойство ScaleCrop
            properties.ScaleCrop = true;
            
            // Отобразить значение свойства ScaleCrop
            Console.WriteLine("ScaleCrop property value: " + properties.ScaleCrop);
            
            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


