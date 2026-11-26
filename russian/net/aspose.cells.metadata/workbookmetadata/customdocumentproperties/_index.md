---
title: "WorkbookMetadata.CustomDocumentProperties"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookMetadata. Возвращает коллекцию DocumentProperty, представляющую все пользовательские свойства документа электронной таблицы"
type: docs
url: /ru/net/aspose.cells.metadata/workbookmetadata/customdocumentproperties/
---
## WorkbookMetadata.CustomDocumentProperties property

Возвращает коллекцию [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/), представляющую все пользовательские свойства документа электронной таблицы.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class WorkbookMetadataPropertyCustomDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Пути источника и назначения
            string sourcePath = "example.xlsx";
            string destPath = "output.xlsx";

            // Создать параметры метаданных для свойств документа
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            
            // Инициализировать метаданные рабочей книги
            WorkbookMetadata meta = new WorkbookMetadata(sourcePath, options);
            
            // Добавить пользовательское свойство документа
            meta.CustomDocumentProperties.Add("Author", "John Doe");
            
            // Сохранить книгу с метаданными
            meta.Save(destPath);
            
            // Проверить пользовательское свойство
            Workbook workbook = new Workbook(destPath);
            Console.WriteLine("Custom Property Value: " + 
                workbook.CustomDocumentProperties["Author"].Value);
        }
    }
}
```

### См. также

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


