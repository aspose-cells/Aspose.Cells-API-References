---
title: "CustomDocumentPropertyCollection.AddLinkToContent"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CustomDocumentPropertyCollection. Создаёт новое пользовательское свойство документа, которое связывается с содержимым"
type: docs
url: /ru/net/aspose.cells.properties/customdocumentpropertycollection/addlinktocontent/
---
## CustomDocumentPropertyCollection.AddLinkToContent method

Создаёт новое пользовательское свойство документа, которое связывается с содержимым.

```csharp
public DocumentProperty AddLinkToContent(string name, string source)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя свойства. |
| источник | String | Источник свойства. Это должно быть имя именованного диапазона. |

### Возвращаемое значение

Недавно созданный объект свойства.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodAddLinkToContentWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите значение в ячейку A1, которое будет связано
            worksheet.Cells["A1"].PutValue("Linked Cell Value");

            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
            
            // Добавьте обычное свойство для сравнения
            customProperties.Add("RegularProperty", "Static Value");
            
            // Добавьте связанное свойство
            customProperties.AddLinkToContent("LinkedProperty", "Sheet1!A1");
            
            // Обновите связанное значение
            customProperties.UpdateLinkedRange();

            // Отобразите свойства
            Console.WriteLine($"Regular Property: {customProperties["RegularProperty"].Value}");
            Console.WriteLine($"Linked Property: {customProperties["LinkedProperty"].Value}");

            workbook.Save("LinkedPropertyExample.xlsx");
        }
    }
}
```

### См. также

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


