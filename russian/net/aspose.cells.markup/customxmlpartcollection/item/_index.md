---
title: "CustomXmlPartCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CustomXmlPartCollection. Возвращает элемент по указанному индексу"
type: docs
url: /ru/net/aspose.cells.markup/customxmlpartcollection/item/
---
## CustomXmlPartCollection indexer

Получает элемент по указанному индексу.

```csharp
public CustomXmlPart this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class CustomXmlPartCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите доступ к CustomXmlPartCollection напрямую из Workbook
            CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;
            
            // Пример XML‑данных
            string xmlData = "<root><item>Test Data</item></root>";
            byte[] xmlBytes = System.Text.Encoding.UTF8.GetBytes(xmlData);
            
            // Добавить пользовательскую часть XML
            int index = customXmlParts.Add(xmlBytes, null);
            
            // Получить доступ к элементу с помощью свойства Item
            CustomXmlPart part = customXmlParts[index];
            
            // Отобразить идентификатор пользовательской части XML
            Console.WriteLine("Custom XML Part ID: " + part.ID);
            
            // Получить XML‑данные из части
            string retrievedXml = System.Text.Encoding.UTF8.GetString(part.Data);
            Console.WriteLine("XML Content: " + retrievedXml);
            
            // Сохраните книгу
            workbook.Save("CustomXmlPartDemo.xlsx");
        }
    }
}
```

### См. также

* class [CustomXmlPart](../../customxmlpart/)
* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


