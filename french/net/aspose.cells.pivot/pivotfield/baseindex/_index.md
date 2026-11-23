---
title: "PivotField.BaseIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Représente l’index dans les champs pivot source"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/baseindex/
---
## PivotField.BaseIndex property

Représente l'index dans les champs pivot source.

```csharp
public int BaseIndex { get; set; }
```

### Remarques

NOTE: Ce mutateur de cette propriété est maintenant obsolète. Ce mutateur de cette propriété sera supprimé 12 mois plus tard à compter de septembre 2026. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyBaseIndexDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[wb.Worksheets.Add()];
            ws.Name = "PivotData";
            
            // Données d'exemple
            ws.Cells["A1"].PutValue("Category");
            ws.Cells["B1"].PutValue("Quarter");
            ws.Cells["C1"].PutValue("Sales");
            
            ws.Cells["A2"].PutValue("Electronics");
            ws.Cells["A3"].PutValue("Electronics");
            ws.Cells["A4"].PutValue("Clothing");
            ws.Cells["A5"].PutValue("Clothing");
            
            ws.Cells["B2"].PutValue("Q1");
            ws.Cells["B3"].PutValue("Q2");
            ws.Cells["B4"].PutValue("Q1");
            ws.Cells["B5"].PutValue("Q2");
            
            ws.Cells["C2"].PutValue(1000);
            ws.Cells["C3"].PutValue(1200);
            ws.Cells["C4"].PutValue(800);
            ws.Cells["C5"].PutValue(900);

            // Créer un tableau croisé dynamique - corrigé en obtenant le PivotTable depuis l’index
            int pivotIndex = ws.PivotTables.Add("=PivotData!A1:C5", "E3", "PivotTable1");
            PivotTable pt = ws.PivotTables[pivotIndex];
            
            // Ajouter le champ de ligne
            int rowIndex = pt.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pt.RowFields[rowIndex];
            
            // Ajouter un champ de colonne (sera utilisé comme champ de base)
            int colIndex = pt.AddFieldToArea(PivotFieldType.Column, "Quarter");
            PivotField quarterField = pt.ColumnFields[colIndex];
            
            // Ajouter un champ de données avec un calcul normal
            int dataIndex = pt.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pt.DataFields[dataIndex];
            dataField.Function = ConsolidationFunction.Sum;
            
            // Ajouter un deuxième champ de données affichant la différence par rapport au trimestre précédent
            int diffIndex = pt.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField diffField = pt.DataFields[diffIndex];
            diffField.DisplayName = "QoQ Difference";
            diffField.ShowValuesAs(
                PivotFieldDataDisplayFormat.DifferenceFrom, 
                quarterField.BaseIndex, 
                PivotItemPositionType.Previous,
                0);
            
            // Calculer et enregistrer
            wb.CalculateFormula();
            wb.Save("PivotTableWithBaseIndexDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


