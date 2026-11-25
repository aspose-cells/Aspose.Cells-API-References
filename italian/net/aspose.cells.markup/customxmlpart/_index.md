---
title: "Classe CustomXmlPart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Markup.CustomXmlPart. Rappresenta una parte di archiviazione dati XML personalizzata Custom XML Data Storage Part all'interno di un pacchetto"
type: docs
url: /it/net/aspose.cells.markup/customxmlpart/
---
## CustomXmlPart class

Rappresenta una parte di archiviazione dati XML personalizzata (dati XML personalizzati all'interno di un pacchetto).

```csharp
public class CustomXmlPart
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Data](../../aspose.cells.markup/customxmlpart/data/) { get; set; } | Ottiene o imposta il contenuto XML di questa Custom XML Data Storage Part. |
| [ID](../../aspose.cells.markup/customxmlpart/id/) { get; set; } | Ottiene e imposta l'ID della parte XML personalizzata. |
| [SchemaData](../../aspose.cells.markup/customxmlpart/schemadata/) { get; set; } | Ottiene o imposta il contenuto XML di questa Custom XML Schema Data Storage Part. |

### Esempi

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

### Vedi anche

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


