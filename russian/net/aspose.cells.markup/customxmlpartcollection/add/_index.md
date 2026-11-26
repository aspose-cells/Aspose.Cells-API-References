---
title: "CustomXmlPartCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CustomXmlPartCollection. Добавляет элемент в коллекцию"
type: docs
url: /ru/net/aspose.cells.markup/customxmlpartcollection/add/
---
## CustomXmlPartCollection.Add method

Добавляет элемент в коллекцию.

```csharp
public int Add(byte[] data, byte[] schemaData)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| данные | Byte[] | XML‑содержимое этой части Custom XML Data Storage Part. |
| schemaData | Byte[] | Набор XML‑схем, связанных с этой пользовательской XML‑частью. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;
    using System.Text;

    public class CustomXmlPartCollectionMethodAddWithByteByteDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите CustomXmlPartCollection напрямую из рабочей книги
            CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;
            
            // Подготовьте XML‑данные и схему в виде массивов байтов
            string xmlData = "<root><item>Test Data</item></root>";
            string schemaData = "<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'><xs:element name='root'><xs:complexType><xs:sequence><xs:element name='item' type='xs:string'/></xs:sequence></xs:complexType></xs:element></xs:schema>";
            
            byte[] xmlBytes = Encoding.UTF8.GetBytes(xmlData);
            byte[] schemaBytes = Encoding.UTF8.GetBytes(schemaData);

            try
            {
                // Вызовите метод Add с параметрами массивов байтов
                int index = customXmlParts.Add(xmlBytes, schemaBytes);
                
                Console.WriteLine($"Custom XML part added successfully at index: {index}");
                
                // Сохраните рабочую книгу, чтобы продемонстрировать эффект
                workbook.Save("CustomXmlPartAddDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding custom XML part: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


