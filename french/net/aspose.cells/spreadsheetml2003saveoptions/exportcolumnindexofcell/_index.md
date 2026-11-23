---
title: "SpreadsheetML2003SaveOptions.ExportColumnIndexOfCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SpreadsheetML2003SaveOptions. La valeur par défaut est false, cela signifie que l'index de colonne sera ignoré si la cellule est contiguë à la cellule précédente"
type: docs
url: /fr/net/aspose.cells/spreadsheetml2003saveoptions/exportcolumnindexofcell/
---
## SpreadsheetML2003SaveOptions.ExportColumnIndexOfCell property

La valeur par défaut est false, cela signifie que l'index de colonne sera ignoré si la cellule est contiguë à la cellule précédente.

```csharp
public bool ExportColumnIndexOfCell { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyExportColumnIndexOfCellDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            
            // Créer des options d'enregistrement avec ExportColumnIndexOfCell activé
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            saveOptions.ExportColumnIndexOfCell = true;
            
            // Enregistrer le classeur avec les informations d'index de colonne
            workbook.Save("output_with_column_index.xml", saveOptions);
            
            Console.WriteLine("File saved with column index information.");
        }
    }
}
```

### Voir aussi

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


