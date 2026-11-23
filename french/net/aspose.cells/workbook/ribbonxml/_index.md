---
title: "Workbook.RibbonXml"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Obtient et définit le fichier XML qui définit l'interface du ruban"
type: docs
url: /fr/net/aspose.cells/workbook/ribbonxml/
---
## Workbook.RibbonXml property

Obtient et définit le fichier XML qui définit l'interface Ribbon.

```csharp
public string RibbonXml { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyRibbonXmlDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Exemple de XML du ruban pour personnaliser le ruban
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

            // Définir la propriété RibbonXml
            workbook.RibbonXml = ribbonXml;

            // Enregistrez le classeur
            workbook.Save("output.xlsm");

            // Vérifier la propriété RibbonXml
            Console.WriteLine("RibbonXml is set: " + (workbook.RibbonXml != null));
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


