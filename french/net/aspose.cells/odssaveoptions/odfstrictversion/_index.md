---
title: "OdsSaveOptions.OdfStrictVersion"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OdsSaveOptions. Obtient et définit la version ODF"
type: docs
url: /fr/net/aspose.cells/odssaveoptions/odfstrictversion/
---
## OdsSaveOptions.OdfStrictVersion property

Obtient et définit la version ODF.

```csharp
public OpenDocumentFormatVersionType OdfStrictVersion { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsPropertyOdfStrictVersionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("ODF Version Demo");

            // Créer des options d’enregistrement ODS
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            
            // Définir la version ODF à 1.2
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;

            // Enregistrer avec la version ODF spécifiée
            workbook.Save("OdfVersion12.ods", saveOptions);

            // Passer à la version ODF 1.3
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf13;
            workbook.Save("OdfVersion13.ods", saveOptions);
        }
    }
}
```

### Voir aussi

* enum [OpenDocumentFormatVersionType](../../../aspose.cells.ods/opendocumentformatversiontype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


