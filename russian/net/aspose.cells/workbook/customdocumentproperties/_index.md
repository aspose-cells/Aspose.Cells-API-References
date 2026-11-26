---
title: "Workbook.CustomDocumentProperties"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Возвращает коллекцию DocumentProperty, представляющую все пользовательские свойства документа электронной таблицы"
type: docs
url: /ru/net/aspose.cells/workbook/customdocumentproperties/
---
## Workbook.CustomDocumentProperties property

Возвращает коллекцию [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/), представляющую все пользовательские свойства документа электронной таблицы.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyCustomDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить пользовательские свойства документа
            workbook.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.CustomDocumentProperties.Add("Created Date", DateTime.Now);
            workbook.CustomDocumentProperties.Add("Revision", 1);
            workbook.CustomDocumentProperties.Add("Approved", true);
            
            // Доступ и отображение пользовательских свойств
            Console.WriteLine("Custom Document Properties:");
            foreach (Aspose.Cells.Properties.DocumentProperty prop in workbook.CustomDocumentProperties)
            {
                Console.WriteLine($"{prop.Name}: {prop.Value} ({prop.Type})");
            }
            
            // Сохраните книгу
            workbook.Save("CustomDocumentPropertiesDemo.xlsx");
        }
    }
}
```

### См. также

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


