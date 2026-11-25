---
title: "Workbook.RibbonXml"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Workbook. Ottiene e imposta il file XML che definisce l'interfaccia Ribbon"
type: docs
url: /it/net/aspose.cells/workbook/ribbonxml/
---
## Workbook.RibbonXml property

Ottiene e imposta il file XML che definisce l'interfaccia Ribbon UI.

```csharp
public string RibbonXml { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyRibbonXmlDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Esempio di XML Ribbon per personalizzare il ribbon
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

            // Imposta la proprietà RibbonXml
            workbook.RibbonXml = ribbonXml;

            // Salva la cartella di lavoro
            workbook.Save("output.xlsm");

            // Verifica la proprietà RibbonXml
            Console.WriteLine("RibbonXml is set: " + (workbook.RibbonXml != null));
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


