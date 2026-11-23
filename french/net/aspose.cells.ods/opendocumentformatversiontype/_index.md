---
title: "Enum OpenDocumentFormatVersionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Ods.OpenDocumentFormatVersionType enum. type de version Open Document Format"
type: docs
url: /fr/net/aspose.cells.ods/opendocumentformatversiontype/
---
## OpenDocumentFormatVersionType enumeration

Type de version du format Open Document.

```csharp
public enum OpenDocumentFormatVersionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Aucun strict. |
| Odf11 | `1` | ODF Version 1.1 |
| Odf12 | `2` | ODF Version 1.2 |
| Odf13 | `3` | ODF Version 1.3 |
| Odf14 | `4` | ODF Version 1.4 |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OpenDocumentFormatVersionTypeDemo
    {
        public static void OpenDocumentFormatVersionTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);

            // Créer OdsSaveOptions et définir la version ODF
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;

            // Enregistrer le classeur au format ODS avec la version ODF spécifiée
            workbook.Save("OpenDocumentFormatVersionTypeExample.ods", saveOptions);

            Console.WriteLine("Workbook saved successfully with ODF version 1.2.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


