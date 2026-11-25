---
title: "XmlSaveOptions.XmlMapName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XmlSaveOptions. Indica se esportare la mappa xml nel file"
type: docs
url: /it/net/aspose.cells/xmlsaveoptions/xmlmapname/
---
## XmlSaveOptions.XmlMapName property

Indica se esportare la mappa XML nel file.

```csharp
public string XmlMapName { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyXmlMapNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Inserisci alcuni dati nel foglio di lavoro
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);

            // Crea una mappa XML e aggiungila alla cartella di lavoro
            int mapIndex = workbook.Worksheets.XmlMaps.Add("<Schema><Element><Product/><Price/></Element></Schema>");
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[mapIndex];
            xmlMap.Name = "ProductDataMap";

            // Crea XmlSaveOptions e imposta XmlMapName
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.XmlMapName = "ProductDataMap";

            // Salva la cartella di lavoro con la mappatura XML
            workbook.Save("XmlWithMapping.xml", saveOptions);
        }
    }
}
```

### Vedi anche

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


