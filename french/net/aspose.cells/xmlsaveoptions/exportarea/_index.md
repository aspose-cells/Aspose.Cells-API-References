---
title: "XmlSaveOptions.ExportArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété XmlSaveOptions. Obtient ou définit la plage d'exportation"
type: docs
url: /fr/net/aspose.cells/xmlsaveoptions/exportarea/
---
## XmlSaveOptions.ExportArea property

Obtient ou définit la plage d'exportation.

```csharp
public CellArea ExportArea { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir les données dans la feuille de calcul
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Créer XmlSaveOptions et définir ExportArea
            XmlSaveOptions saveOptions = new XmlSaveOptions
            {
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 }
            };

            // Enregistrer uniquement la zone spécifiée en XML
            workbook.Save("ExportAreaDemo.xml", saveOptions);
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


