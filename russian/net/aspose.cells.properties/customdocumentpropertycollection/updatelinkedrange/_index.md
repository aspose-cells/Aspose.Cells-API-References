---
title: "CustomDocumentPropertyCollection.UpdateLinkedRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CustomDocumentPropertyCollection. Обновляет все диапазоны, связанные с пользовательскими свойствами, используя значение пользовательского свойства документа для обновления значения ячейки связанного диапазона"
type: docs
url: /ru/net/aspose.cells.properties/customdocumentpropertycollection/updatelinkedrange/
---
## CustomDocumentPropertyCollection.UpdateLinkedRange method

Обновляет все диапазоны, связанные с пользовательскими свойствами (использует значение пользовательского свойства документа для обновления значения ячейки связанного диапазона).

```csharp
public void UpdateLinkedRange()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodUpdateLinkedRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите значение в ячейку A1, которое будет связано
            worksheet.Cells["A1"].PutValue("Linked Cell Value");

            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
            
            // Добавьте связанное свойство
            customProperties.AddLinkToContent("LinkedRange", "Sheet1!A1");
            
            // Обновить все связанные свойства
            customProperties.UpdateLinkedRange();
            
            // Получить и отобразить значение связанного свойства
            DocumentProperty linkedProp = customProperties["LinkedRange"];
            Console.WriteLine($"Linked Property Value: {linkedProp.Value}");

            // Сохраните книгу
            workbook.Save("LinkedRangeExample.xlsx");
        }
    }
}
```

### См. также

* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


