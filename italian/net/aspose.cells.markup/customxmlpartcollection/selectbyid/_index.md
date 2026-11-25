---
title: "CustomXmlPartCollection.SelectByID"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CustomXmlPartCollection. Ottiene un elemento per ID"
type: docs
url: /it/net/aspose.cells.markup/customxmlpartcollection/selectbyid/
---
## CustomXmlPartCollection.SelectByID method

Ottiene un elemento per ID.

```csharp
public CustomXmlPart SelectByID(string id)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| id | String | Contiene il GUID per la parte XML personalizzata. |

### Esempi

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

### Vedi anche

* class [CustomXmlPart](../../customxmlpart/)
* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


