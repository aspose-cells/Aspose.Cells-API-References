---
title: "Enum OoxmlCompliance"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.OoxmlCompliance enum. Permet de spécifier quelle spécification OOXML sera utilisée lors de l'enregistrement au format Xlsx"
type: docs
url: /fr/net/aspose.cells/ooxmlcompliance/
---
## OoxmlCompliance enumeration

Permet de spécifier quelle spécification OOXML sera utilisée lors de l'enregistrement au format Xlsx.

```csharp
public enum OoxmlCompliance
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Ecma376_2006 | `0` | ECMA-376 1re édition, 2006. |
| Iso29500_2008_Strict | `1` | Niveau de conformité strict ISO/IEC 29500 :2008. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlComplianceDemo
    {
        public static void OoxmlComplianceExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder aux paramètres du classeur
            WorkbookSettings settings = workbook.Settings;

            // Définir le niveau de conformité OOXML sur ISO/IEC 29500 :2008 Strict
            settings.Compliance = OoxmlCompliance.Iso29500_2008_Strict;

            // Ajouter des données à la feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, World!");

            // Enregistrer le classeur avec le niveau de conformité OOXML spécifié
            workbook.Save("OoxmlComplianceExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


