---
title: "OoxmlSaveOptions.WpsCompatibility"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OoxmlSaveOptions. Indique s'il faut rendre le xls plus compatible avec WPS"
type: docs
url: /fr/net/aspose.cells/ooxmlsaveoptions/wpscompatibility/
---
## OoxmlSaveOptions.WpsCompatibility property

Indique s’il faut rendre le xls plus compatible avec WPS.

```csharp
[Obsolete("Use WorkbookSetting.WpsCompatibility property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool WpsCompatibility { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété WorkbookSetting.WpsCompatibility. Cette méthode sera supprimée 12 mois plus tard, à compter de décembre 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyWpsCompatibilityDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez à la première feuille de calcul et ajoutez des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test WPS Compatibility");
            
            // Créer des options d'enregistrement OOXML et activer la compatibilité WPS
            OoxmlSaveOptions options = new OoxmlSaveOptions();
            options.WpsCompatibility = true;
            
            // Enregistrer le classeur avec la compatibilité WPS
            workbook.Save("output_with_wps_compatibility.xlsx", options);
            
            Console.WriteLine("Workbook saved with WPS compatibility enabled.");
        }
    }
}
```

### Voir aussi

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


