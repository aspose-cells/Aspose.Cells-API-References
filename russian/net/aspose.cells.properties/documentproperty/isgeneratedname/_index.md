---
title: "DocumentProperty.IsGeneratedName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DocumentProperty. Возвращает true, если у этого свойства нет имени в хранилище OLE2 и уникальное имя было сгенерировано только для публичного API"
type: docs
url: /ru/net/aspose.cells.properties/documentproperty/isgeneratedname/
---
## DocumentProperty.IsGeneratedName property

Возвращает true, если у этого свойства нет имени в хранилище OLE2 и уникальное имя было сгенерировано только для публичного API.

```csharp
public bool IsGeneratedName { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyPropertyIsGeneratedNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к встроенным свойствам документа
            DocumentPropertyCollection properties = workbook.Worksheets.BuiltInDocumentProperties;
            
            // Получите доступ к пользовательским свойствам документа для добавления
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Добавить пользовательское свойство
            DocumentProperty customProperty = customProperties.Add("CustomProperty", "Test Value");
            
            // Отобразите IsGeneratedName для встроенного свойства
            DocumentProperty authorProperty = properties["Author"];
            Console.WriteLine("Author property IsGeneratedName: " + authorProperty.IsGeneratedName);
            
            // Отобразите IsGeneratedName для пользовательского свойства
            Console.WriteLine("Custom property IsGeneratedName: " + customProperty.IsGeneratedName);

            // Создайте сценарий, в котором у свойства может быть сгенерированное имя
            // (Примечание: На практике IsGeneratedName доступен только для чтения и устанавливается внутренне Aspose.Cells)
            DocumentProperty generatedNameProperty = properties["_PID_GUID"];
            if (generatedNameProperty != null)
            {
                Console.WriteLine("Generated name property IsGeneratedName: " + generatedNameProperty.IsGeneratedName);
            }

            // Сохраните книгу
            workbook.Save("PropertyIsGeneratedNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


