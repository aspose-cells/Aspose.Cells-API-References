---
title: "Workbook.CustomXmlParts"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Workbook. Rappresenta una Custom XML Data Storage Part con dati XML personalizzati all'interno di un pacchetto"
type: docs
url: /it/net/aspose.cells/workbook/customxmlparts/
---
## Workbook.CustomXmlParts property

Rappresenta una parte di archiviazione dati XML personalizzata (dati XML personalizzati all'interno di un pacchetto).

```csharp
public CustomXmlPartCollection CustomXmlParts { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            
            // Definisci i dati XML e lo schema
            string xmlData = "<MyXmlData1 xmlns=\"http://my.namespace.com\"/>";
            string xmlSchema = "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>" +
                "<ds:datastoreItem ds:itemID=\"{1D3CF2F4-9155-40AE-99F6-33298D217F89}\" xmlns:ds=\"http://schemas.openxmlformats.org/officeDocument/2006/customXml\">" +
                    "<ds:schemaRefs>" +
                        "<ds:schemaRef ds:uri=\"http://my.namespace.com\"/>" +
                    "</ds:schemaRefs>" +
                "</ds:datastoreItem>";

            // Aggiungi una parte XML personalizzata al workbook
            wb.CustomXmlParts.Add(Encoding.UTF8.GetBytes(xmlData), Encoding.UTF8.GetBytes(xmlSchema));

            // Salva e ricarica il workbook
            string outputPath = "output.xlsx";
            wb.Save(outputPath);
            
            Workbook loadedWb = new Workbook(outputPath);
            
            // Mostra il conteggio delle parti XML personalizzate
            Console.WriteLine($"Number of custom XML parts: {loadedWb.CustomXmlParts.Count}");
        }
    }
}
```

### Vedi anche

* class [CustomXmlPartCollection](../../../aspose.cells.markup/customxmlpartcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


