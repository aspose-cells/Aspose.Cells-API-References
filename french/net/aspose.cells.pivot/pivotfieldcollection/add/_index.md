---
title: "PivotFieldCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotFieldCollection. Ajoute un objet PivotField au type spécifique PivotFields"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfieldcollection/add/
---
## PivotFieldCollection.Add method

Ajoute un objet PivotField au type spécifique PivotFields.

```csharp
public int Add(PivotField pivotField)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pivotField | PivotField | un objet PivotField. |

### Valeur de retour

l'indice de l'objet PivotField dans ces PivotFields.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionMethodAddWithPivotFieldDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("sample_pivot_table.xlsx");
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder au premier tableau croisé dynamique
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Actualiser les données du tableau croisé dynamique
            pivotTable.RefreshData();
            
            // Ajouter un champ de données à la zone des champs de colonne en utilisant la méthode Add
            pivotTable.ColumnFields.Add(pivotTable.DataField);
            
            // Calculer les données du tableau croisé dynamique
            pivotTable.CalculateData();
            
            // Enregistrez le classeur
            workbook.Save("output_pivot_table.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


