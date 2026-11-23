---
title: "PivotField.NonAutoSortDefault"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Indique si une opération de tri qui sera appliquée à ce champ pivot est une opération de tri automatique ou un tri de données simple"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/nonautosortdefault/
---
## PivotField.NonAutoSortDefault property

Indique si une opération de tri qui sera appliquée à ce champ pivot est une opération de tri automatique ou un tri de données simple.

```csharp
[Obsolete("Use !PivotField.SortSetting.IsSimpleSort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool NonAutoSortDefault { get; set; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété !PivotField.SortSetting.IsSimpleSort. Cette méthode sera supprimée 12 mois plus tard, depuis septembre 2026. Aspose s’excuse pour tout inconvénient que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyNonAutoSortDefaultDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accédez à la première feuille de calcul et au tableau croisé dynamique
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Accédez au premier champ de ligne dans le tableau croisé dynamique
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Définissez la propriété NonAutoSortDefault sur true
            pivotField.NonAutoSortDefault = true;
            
            // Afficher la valeur de la propriété
            Console.WriteLine("NonAutoSortDefault property value: " + pivotField.NonAutoSortDefault);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


