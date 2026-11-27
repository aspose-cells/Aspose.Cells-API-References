---
title: "Workbook.CustomXmlParts"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook‑egenskap. Representerar en Custom XML Data Storage Part‑custom XML‑data inom ett paket"
type: docs
url: /sv/net/aspose.cells/workbook/customxmlparts/
---
## Workbook.CustomXmlParts property

Representerar en anpassad XML‑databasdel (anpassad XML‑data inom ett paket).

```csharp
public CustomXmlPartCollection CustomXmlParts { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            
            // Definiera XML‑data och schema
            string xmlData = "<MyXmlData1 xmlns=\"http://my.namespace.com\"/>";
            string xmlSchema = "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>" +
                "<ds:datastoreItem ds:itemID=\"{1D3CF2F4-9155-40AE-99F6-33298D217F89}\" xmlns:ds=\"http://schemas.openxmlformats.org/officeDocument/2006/customXml\">" +
                    "<ds:schemaRefs>" +
                        "<ds:schemaRef ds:uri=\"http://my.namespace.com\"/>" +
                    "</ds:schemaRefs>" +
                "</ds:datastoreItem>";

            // Lägg till anpassad XML‑del i arbetsboken
            wb.CustomXmlParts.Add(Encoding.UTF8.GetBytes(xmlData), Encoding.UTF8.GetBytes(xmlSchema));

            // Spara och ladda om arbetsboken
            string outputPath = "output.xlsx";
            wb.Save(outputPath);
            
            Workbook loadedWb = new Workbook(outputPath);
            
            // Visa antalet anpassade XML‑delar
            Console.WriteLine($"Number of custom XML parts: {loadedWb.CustomXmlParts.Count}");
        }
    }
}
```

### Se även

* class [CustomXmlPartCollection](../../../aspose.cells.markup/customxmlpartcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


