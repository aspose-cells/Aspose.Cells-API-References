---
title: "PivotField.OriginalItems"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Obtenir les éléments de base originaux"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/originalitems/
---
## PivotField.OriginalItems property

Obtient les éléments de base originaux;

```csharp
public string[] OriginalItems { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyOriginalItemsDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("AsposeGroupedField2.xlsx");
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder au premier tableau croisé dynamique
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Accéder au premier champ de ligne
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Afficher les éléments originaux et les éléments groupés
            Console.WriteLine("Original Item[0]: " + pivotField.OriginalItems[0]);
            Console.WriteLine("Grouped Item[0]: " + pivotField.Items[0]);
            
            // Enregistrer le classeur modifié
            workbook.Save("PivotFieldOriginalItemsDemo_Output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


