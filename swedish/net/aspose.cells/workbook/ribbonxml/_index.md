---
title: "Workbook.RibbonXml"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook‑egenskap. Hämtar och anger XML‑filen som definierar Ribbon‑UI"
type: docs
url: /sv/net/aspose.cells/workbook/ribbonxml/
---
## Workbook.RibbonXml property

Hämtar och anger XML-filen som definierar Ribbon‑UI.

```csharp
public string RibbonXml { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyRibbonXmlDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Exempel‑ribbon‑XML för att anpassa ribbon
            string ribbonXml = 
                "<customUI xmlns=\"http://schemas.microsoft.com/office/2006/01/customui\">" +
                "  <ribbon>" +
                "    <tabs>" +
                "      <tab id=\"customTab\" label=\"My Tab\">" +
                "        <group id=\"customGroup\" label=\"My Group\">" +
                "          <button id=\"customButton\" label=\"My Button\" size=\"large\" />" +
                "        </group>" +
                "      </tab>" +
                "    </tabs>" +
                "  </ribbon>" +
                "</customUI>";

            // Ställ in RibbonXml-egenskapen
            workbook.RibbonXml = ribbonXml;

            // Spara arbetsboken
            workbook.Save("output.xlsm");

            // Verifiera RibbonXml-egenskapen
            Console.WriteLine("RibbonXml is set: " + (workbook.RibbonXml != null));
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


