---
title: "DocumentProperty.IsLinkedToContent"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DocumentProperty. Указывает, связано ли это свойство с содержимым"
type: docs
url: /ru/net/aspose.cells.properties/documentproperty/islinkedtocontent/
---
## DocumentProperty.IsLinkedToContent property

Указывает, связано ли это свойство с содержимым

```csharp
public bool IsLinkedToContent { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyIsLinkedToContentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить примерные данные в ячейки
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Company Name";
            worksheet.Cells["B1"].Value = "Company Address";

            // Создайте связанные пользовательские свойства документа
            workbook.CustomDocumentProperties.AddLinkToContent("Company", "A1");
            workbook.CustomDocumentProperties.AddLinkToContent("Address", "B1");

            // Получите и проверьте свойство IsLinkedToContent
            DocumentProperty companyProp = workbook.CustomDocumentProperties["Company"];
            Console.WriteLine($"Is 'Company' property linked to content: {companyProp.IsLinkedToContent}");
            Console.WriteLine($"Linked source: {companyProp.Source}");
            Console.WriteLine($"Current value: {companyProp.Value}");

            // Обновите значение ячейки и обновите связанные свойства
            worksheet.Cells["A1"].Value = "Updated Company Name";
            workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();

            // Проверьте, что свойство было обновлено
            Console.WriteLine($"Updated value: {companyProp.Value}");

            // Сохраните книгу
            workbook.Save("LinkedPropertiesDemo.xlsx");
        }
    }
}
```

### См. также

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


