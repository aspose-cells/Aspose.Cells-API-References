---
title: "Workbook.CustomXmlParts"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Eigenschaft. Stellt einen Custom XML Data Storage Part dar, benutzerdefinierte XML-Daten innerhalb eines Pakets"
type: docs
url: /de/net/aspose.cells/workbook/customxmlparts/
---
## Workbook.CustomXmlParts property

Stellt einen benutzerdefinierten XML‑Datenspeicherteil dar (benutzerdefinierte XML‑Daten innerhalb eines Pakets).

```csharp
public CustomXmlPartCollection CustomXmlParts { get; }
```

### Beispiele

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyCustomXmlPartsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            
            // Definiere XML-Daten und Schema
            string xmlData = "<MyXmlData1 xmlns=\"http://my.namespace.com\"/>";
            string xmlSchema = "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>" +
                "<ds:datastoreItem ds:itemID=\"{1D3CF2F4-9155-40AE-99F6-33298D217F89}\" xmlns:ds=\"http://schemas.openxmlformats.org/officeDocument/2006/customXml\">" +
                    "<ds:schemaRefs>" +
                        "<ds:schemaRef ds:uri=\"http://my.namespace.com\"/>" +
                    "</ds:schemaRefs>" +
                "</ds:datastoreItem>";

            // Füge dem Workbook einen benutzerdefinierten XML-Part hinzu
            wb.CustomXmlParts.Add(Encoding.UTF8.GetBytes(xmlData), Encoding.UTF8.GetBytes(xmlSchema));

            // Speichere das Workbook und lade es erneut
            string outputPath = "output.xlsx";
            wb.Save(outputPath);
            
            Workbook loadedWb = new Workbook(outputPath);
            
            // Zeige die Anzahl der benutzerdefinierten XML-Parts an
            Console.WriteLine($"Number of custom XML parts: {loadedWb.CustomXmlParts.Count}");
        }
    }
}
```

### Siehe auch

* class [CustomXmlPartCollection](../../../aspose.cells.markup/customxmlpartcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


