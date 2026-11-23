---
title: "PivotFieldCollection.AddByBaseIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotFieldCollection. Ajoute un objet PivotField au type spécifique PivotFields"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfieldcollection/addbybaseindex/
---
## PivotFieldCollection.AddByBaseIndex method

Ajoute un objet PivotField au type spécifique PivotFields.

```csharp
public int AddByBaseIndex(int baseFieldIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| baseFieldIndex | Int32 | index du champ dans les PivotFields de base. |

### Valeur de retour

l'indice de l'objet PivotField dans ces PivotFields.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionMethodAddByBaseIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Données d'exemple
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Year";
            worksheet.Cells["B2"].Value = 2022;
            worksheet.Cells["B3"].Value = 2023;
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["C2"].Value = 1000;
            worksheet.Cells["C3"].Value = 2000;

            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:C3", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Ajoutez les champs initiaux
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Ajoutez le champ Année à la zone de lignes en utilisant AddByBaseIndex
            int newIndex = pivotTable.RowFields.AddByBaseIndex(1);
            Console.WriteLine("Added field at index: " + newIndex);

            workbook.Save("PivotFieldAddByBaseIndexDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


