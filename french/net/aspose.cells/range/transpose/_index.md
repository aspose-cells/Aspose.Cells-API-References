---
title: "Range.Transpose"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Transpose fait pivoter les données des lignes aux colonnes ou inversement"
type: docs
url: /fr/net/aspose.cells/range/transpose/
---
## Range.Transpose method

Transposer (faire pivoter) les données des lignes aux colonnes ou inversement.

```csharp
public void Transpose()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodTransposeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplissez des données d'exemple dans une plage 3x3 (A1:C3)
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(3);
            worksheet.Cells["A2"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["C2"].PutValue(6);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["C3"].PutValue(9);
            
            // Créez une plage (A1:C3)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            
            // Transposez la plage
            range.Transpose();
            
            // Enregistrez le classeur
            workbook.Save("TransposedOutput.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


