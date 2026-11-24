---
title: "XmlSaveOptions.XmlMapName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XmlSaveOptions-Eigenschaft. Gibt an, ob eine XML-Map in die Datei exportiert wird"
type: docs
url: /de/net/aspose.cells/xmlsaveoptions/xmlmapname/
---
## XmlSaveOptions.XmlMapName property

Gibt an, ob die XML‑Map in der Datei exportiert wird.

```csharp
public string XmlMapName { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyXmlMapNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füllen Sie einige Daten im Arbeitsblatt ein
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);

            // Erstelle eine XML-Map und füge sie dem Arbeitsbuch hinzu
            int mapIndex = workbook.Worksheets.XmlMaps.Add("<Schema><Element><Product/><Price/></Element></Schema>");
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[mapIndex];
            xmlMap.Name = "ProductDataMap";

            // Erstelle XmlSaveOptions und setze XmlMapName
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.XmlMapName = "ProductDataMap";

            // Speichere das Arbeitsbuch mit XML-Mapping
            workbook.Save("XmlWithMapping.xml", saveOptions);
        }
    }
}
```

### Siehe auch

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


