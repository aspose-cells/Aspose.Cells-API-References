---
title: "Workbook.RibbonXml"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Eigenschaft. Gibt die XML-Datei zurück und legt sie fest, die das Ribbon-UI definiert"
type: docs
url: /de/net/aspose.cells/workbook/ribbonxml/
---
## Workbook.RibbonXml property

Liest und setzt die XML‑Datei, die die Ribbon‑UI definiert.

```csharp
public string RibbonXml { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyRibbonXmlDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Beispiel-Ribbon-XML zum Anpassen des Ribbons
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

            // Setze die RibbonXml-Eigenschaft
            workbook.RibbonXml = ribbonXml;

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsm");

            // Überprüfe die RibbonXml-Eigenschaft
            Console.WriteLine("RibbonXml is set: " + (workbook.RibbonXml != null));
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


