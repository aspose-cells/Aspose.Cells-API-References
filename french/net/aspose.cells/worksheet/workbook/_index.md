---
title: "Worksheet.Workbook"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Obtient l'objet classeur qui contient cette feuille"
type: docs
url: /fr/net/aspose.cells/worksheet/workbook/
---
## Worksheet.Workbook property

Obtient l'objet classeur qui contient cette feuille.

```csharp
public Workbook Workbook { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyWorkbookDemo
    {
        public static void Run()
        {
            // Créer un classeur source et obtenir une feuille de calcul
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Ajouter des données d'exemple à la feuille de calcul source
            sourceSheet.Cells["A1"].PutValue("Sample Data");
            sourceSheet.Cells["A2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue(200);
            
            // Créer un classeur de destination
            Workbook destWorkbook = new Workbook();
            
            // Copier le thème du classeur source en utilisant la propriété Worksheet.Workbook
            destWorkbook.CopyTheme(sourceSheet.Workbook);
            
            // Accéder à la feuille de calcul de destination et copier les données
            Worksheet destSheet = destWorkbook.Worksheets[0];
            Aspose.Cells.Range sourceRange = sourceSheet.Cells.CreateRange("A1:A3");
            Aspose.Cells.Range destRange = destSheet.Cells.CreateRange("A1:A3");
            
            // Copier les données avec le formatage
            destRange.Copy(sourceRange);
            
            // Enregistrer le classeur de destination
            destWorkbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Workbook](../../workbook/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


