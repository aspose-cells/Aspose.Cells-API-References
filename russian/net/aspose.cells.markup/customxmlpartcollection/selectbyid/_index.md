---
title: "CustomXmlPartCollection.SelectByID"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CustomXmlPartCollection. Получает элемент по идентификатору"
type: docs
url: /ru/net/aspose.cells.markup/customxmlpartcollection/selectbyid/
---
## CustomXmlPartCollection.SelectByID method

Получает элемент по идентификатору.

```csharp
public CustomXmlPart SelectByID(string id)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| id | String | Содержит GUID пользовательской части XML. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class CustomXmlPartCollectionMethodSelectByIDWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook("source.xlsx");
            
            CustomXmlPart part = workbook.CustomXmlParts.SelectByID("2F087CB2-7CA8-43DA-B048-2E2F61F4936F");
            Console.WriteLine("Original ID: " + part.ID);

            string newId = "2F087CB2-7CA8-43DA-B048-2E2F61F0000F";
            part.ID = newId;
            workbook.Save("output.xlsx");

            Workbook reloadedWorkbook = new Workbook("output.xlsx");
            CustomXmlPart reloadedPart = reloadedWorkbook.CustomXmlParts.SelectByID(newId);
            Console.WriteLine("New ID: " + reloadedPart.ID);
        }
    }
}
```

### См. также

* class [CustomXmlPart](../../customxmlpart/)
* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


