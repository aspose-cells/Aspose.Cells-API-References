---
title: "XmlSaveOptions.XmlMapName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XmlSaveOptions egenskap. Anger om xml‑karta exporteras i filen"
type: docs
url: /sv/net/aspose.cells/xmlsaveoptions/xmlmapname/
---
## XmlSaveOptions.XmlMapName property

Anger om XML‑karta exporteras i filen.

```csharp
public string XmlMapName { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyXmlMapNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i några data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);

            // Skapa XML‑karta och lägg till den i arbetsboken
            int mapIndex = workbook.Worksheets.XmlMaps.Add("<Schema><Element><Product/><Price/></Element></Schema>");
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[mapIndex];
            xmlMap.Name = "ProductDataMap";

            // Skapa XmlSaveOptions och ange XmlMapName
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.XmlMapName = "ProductDataMap";

            // Spara arbetsboken med XML‑mappning
            workbook.Save("XmlWithMapping.xml", saveOptions);
        }
    }
}
```

### Se även

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


