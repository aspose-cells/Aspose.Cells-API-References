---
title: "Класс CustomXmlPart"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Markup.CustomXmlPart класс. Представляет часть хранилища пользовательских XML-данных Custom XML Data Storage Part внутри пакета."
type: docs
url: /ru/net/aspose.cells.markup/customxmlpart/
---
## CustomXmlPart class

Представляет часть хранилища пользовательского XML-данных (пользовательские XML‑данные внутри пакета).

```csharp
public class CustomXmlPart
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Data](../../aspose.cells.markup/customxmlpart/data/) { get; set; } | Получает или задает XML‑содержимое этой части хранилища пользовательских XML-данных Custom XML Data Storage Part. |
| [ID](../../aspose.cells.markup/customxmlpart/id/) { get; set; } | Получает и задает идентификатор пользовательской XML‑части. |
| [SchemaData](../../aspose.cells.markup/customxmlpart/schemadata/) { get; set; } | Получает и задает XML‑содержимое этой части хранилища схемы пользовательского XML Custom XML Schema Data Storage Part. |

### Примеры

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class MarkupClassCustomXmlPartDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            CustomXmlPartCollection xmlParts = workbook.CustomXmlParts;

            string xmlData = "<root><item>Sample Data</item></root>";
            byte[] dataBytes = Encoding.UTF8.GetBytes(xmlData);

            string originalId = Guid.NewGuid().ToString();
            int index = xmlParts.Add(dataBytes, null);
            CustomXmlPart newPart = xmlParts[index];
            newPart.ID = originalId;

            Console.WriteLine("Original ID: " + originalId);
            Console.WriteLine("Stored ID: " + newPart.ID);

            string newId = Guid.NewGuid().ToString();
            newPart.ID = newId;
            Console.WriteLine("Updated ID: " + newId);

            workbook.Save("output.xlsx");

            Workbook loadedWorkbook = new Workbook("output.xlsx");
            CustomXmlPart retrievedPart = loadedWorkbook.CustomXmlParts.SelectByID(newId);
            Console.WriteLine("Retrieved ID: " + (retrievedPart != null ? retrievedPart.ID : "Not found"));
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


