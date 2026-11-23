---
title: "PivotTable.CopyStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "PivotTable method. Copie le style nommé d’un autre tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/copystyle/
---
## PivotTable.CopyStyle method

Copie le style nommé d'un autre tableau croisé dynamique.

```csharp
public void CopyStyle(PivotTable pivotTable)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | Tableau croisé dynamique source. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCopyStyleWithPivotTableDemo
    {
        public static void Run()
        {
            // Créer le classeur source avec un tableau croisé dynamique
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            sourceSheet.Cells["A1"].PutValue("Product");
            sourceSheet.Cells["B1"].PutValue("Sales");
            sourceSheet.Cells["A2"].PutValue("A");
            sourceSheet.Cells["B2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue("B");
            sourceSheet.Cells["B3"].PutValue(200);
            
            // Créer le tableau croisé dynamique source (obtenir explicitement l'objet tableau croisé dynamique)
            PivotTable sourcePivotTable = sourceSheet.PivotTables[sourceSheet.PivotTables.Add("PivotTable1", "A1:B3", "C3")];
            sourcePivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            sourcePivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Appliquer le style au tableau croisé dynamique source
            sourcePivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            
            // Créer le classeur de destination avec un tableau croisé dynamique
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Ajouter la même structure de données
            destSheet.Cells["A1"].PutValue("Product");
            destSheet.Cells["B1"].PutValue("Sales");
            destSheet.Cells["A2"].PutValue("A");
            destSheet.Cells["B2"].PutValue(150);
            destSheet.Cells["A3"].PutValue("B");
            destSheet.Cells["B3"].PutValue(250);
            
            // Créer le tableau croisé dynamique de destination (obtenir explicitement l'objet tableau croisé dynamique)
            PivotTable destPivotTable = destSheet.PivotTables[destSheet.PivotTables.Add("PivotTable2", "A1:B3", "C3")];
            destPivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            destPivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Copier le style du tableau croisé dynamique source vers le tableau croisé dynamique de destination
            destPivotTable.CopyStyle(sourcePivotTable);
            
            // Enregistrer le résultat
            destWorkbook.Save("PivotTableStyleCopied.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


