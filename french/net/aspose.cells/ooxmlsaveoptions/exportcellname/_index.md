---
title: "OoxmlSaveOptions.ExportCellName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OoxmlSaveOptions. Indique s'il faut exporter le nom des cellules vers un fichier Excel2007 .xlsx .xlsm .xltx .xltm. Si le fichier de sortie peut être accédé par SQL Server DTS, cette valeur doit être vraie. Mettre la valeur à false augmentera fortement les performances et réduira la taille du fichier lors de la création de gros fichiers. La valeur par défaut est true."
type: docs
url: /fr/net/aspose.cells/ooxmlsaveoptions/exportcellname/
---
## OoxmlSaveOptions.ExportCellName property

Indique si le nom de la cellule doit être exporté vers un fichier Excel2007 .xlsx (.xlsm, .xltx, .xltm). Si le fichier de sortie peut être accédé par SQL Server DTS, cette valeur doit être true. Mettre la valeur à false augmentera considérablement les performances et réduira la taille du fichier lors de la création de gros fichiers. La valeur par défaut est true.

```csharp
public bool ExportCellName { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyExportCellNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Mettre des données dans les cellules
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B2"].PutValue(123);
            
            // Créer des options d'enregistrement XLSX avec ExportCellName activé
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.ExportCellName = true;
            
            // Enregistrer le classeur avec les noms de cellules exportés
            workbook.Save("output_with_cellnames.xlsx", saveOptions);
            
            // Créer d'autres options d'enregistrement avec ExportCellName désactivé (par défaut)
            OoxmlSaveOptions saveOptions2 = new OoxmlSaveOptions();
            
            // Enregistrer le classeur sans exporter les noms de cellules
            workbook.Save("output_without_cellnames.xlsx", saveOptions2);
        }
    }
}
```

### Voir aussi

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


