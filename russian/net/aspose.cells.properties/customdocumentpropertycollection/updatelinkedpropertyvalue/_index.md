---
title: "CustomDocumentPropertyCollection.UpdateLinkedPropertyValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CustomDocumentPropertyCollection. Обновляет значения всех пользовательских свойств, связанных с содержимым, используя значение ячейки связанного диапазона для обновления значения пользовательского свойства"
type: docs
url: /ru/net/aspose.cells.properties/customdocumentpropertycollection/updatelinkedpropertyvalue/
---
## CustomDocumentPropertyCollection.UpdateLinkedPropertyValue method

Обновляет значения всех пользовательских свойств, связанных с содержимым (использует значение ячейки связанного диапазона для обновления значения пользовательского свойства).

```csharp
public void UpdateLinkedPropertyValue()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodUpdateLinkedPropertyValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте некоторые данные в ячейки, которые будут связаны с пользовательскими свойствами
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "InitialValue1";
            worksheet.Cells["B1"].Value = "InitialValue2";

            // Добавьте связанные пользовательские свойства
            workbook.CustomDocumentProperties.AddLinkToContent("CompanyName", "A1");
            workbook.CustomDocumentProperties.AddLinkToContent("Department", "B1");

            // Обновите значения ячеек
            worksheet.Cells["A1"].Value = "UpdatedValue1";
            worksheet.Cells["B1"].Value = "UpdatedValue2";

            // Обновите значения связанных свойств
            workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();

            // Отобразите обновленные значения свойств
            Console.WriteLine("CompanyName: " + workbook.CustomDocumentProperties["CompanyName"].Value);
            Console.WriteLine("Department: " + workbook.CustomDocumentProperties["Department"].Value);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


