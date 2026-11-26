---
title: "CustomXmlPart.Data"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CustomXmlPart. Получает или задает XML‑содержимое этой части Custom XML Data Storage Part"
type: docs
url: /ru/net/aspose.cells.markup/customxmlpart/data/
---
## CustomXmlPart.Data property

Получает или задает XML‑содержимое этой части хранилища пользовательских XML-данных Custom XML Data Storage Part.

```csharp
public byte[] Data { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;
    using System.Text;

    public class CustomXmlPartPropertyDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            byte[] initialData = Encoding.UTF8.GetBytes("<root><data>Initial Value</data></root>");
            int xmlPartIndex = workbook.CustomXmlParts.Add(initialData, null);
            CustomXmlPart xmlPart = workbook.CustomXmlParts[xmlPartIndex];
            
            Console.WriteLine("Current Data value: " + Encoding.UTF8.GetString(xmlPart.Data));

            xmlPart.Data = Encoding.UTF8.GetBytes("<root><data>Modified Value</data></root>");

            workbook.CustomXmlParts.Add(xmlPart.Data, null);
            workbook.Save("CustomXmlPartDataDemo.xlsx");
        }
    }
}
```

### См. также

* class [CustomXmlPart](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


