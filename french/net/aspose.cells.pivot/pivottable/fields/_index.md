---
title: "PivotTable.Fields"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "PivotTable method. Obtient les champs spécifiques par type de champ"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/fields/
---
## PivotTable.Fields method

Obtient les champs spécifiques par type de champ.

```csharp
[Obsolete("Use PivotField.GetFields(PivotFieldType) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotFieldCollection Fields(PivotFieldType fieldType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | le type de champ. |

### Valeur de retour

la collection de champs spécifiques

### Remarques

NOTE : Cette méthode est maintenant obsolète. Veuillez plutôt utiliser la méthode PivotField.GetFields(PivotFieldType). Cette méthode sera supprimée 12 mois plus tard, à partir de mai 2024. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodFieldsWithPivotFieldTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[wb.Worksheets.Add()];
            ws.Name = "Sheet";

            // Données d'exemple
            ws.Cells[0, 0].PutValue("X");
            ws.Cells[0, 1].PutValue("Y");
            ws.Cells[0, 2].PutValue("Data");

            ws.Cells[1, 0].PutValue("A");
            ws.Cells[1, 1].PutValue("C");
            ws.Cells[1, 2].PutValue(10);

            ws.Cells[2, 0].PutValue("A");
            ws.Cells[2, 1].PutValue("D");
            ws.Cells[2, 2].PutValue(25);

            ws.Cells[3, 0].PutValue("B");
            ws.Cells[3, 1].PutValue("C");
            ws.Cells[3, 2].PutValue(30);

            ws.Cells[4, 0].PutValue("B");
            ws.Cells[4, 1].PutValue("D");
            ws.Cells[4, 2].PutValue(45);

            // Créer un tableau croisé dynamique
            PivotTableCollection ptc = ws.PivotTables;
            int index = ptc.Add("=Sheet!A1:C5", "A7", "PivotTable1");
            PivotTable pt = ptc[index];

            // Ajoutez des champs et démontrez la méthode Fields avec PivotFieldType
            int fp = pt.AddFieldToArea(PivotFieldType.Row, "X");
            PivotField rowField = pt.Fields(PivotFieldType.Row)[fp];

            fp = pt.AddFieldToArea(PivotFieldType.Column, "Y");
            PivotField colField = pt.Fields(PivotFieldType.Column)[fp];

            fp = pt.AddFieldToArea(PivotFieldType.Data, "Data");
            PivotField dataField = pt.Fields(PivotFieldType.Data)[fp];

            // Ajoutez un deuxième champ de données avec calcul de pourcentage
            fp = pt.AddFieldToArea(PivotFieldType.Data, "Data");
            dataField = pt.Fields(PivotFieldType.Data)[fp];
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfColumn;

            pt.AddFieldToArea(PivotFieldType.Column, pt.DataField);
            pt.RefreshData();
            pt.CalculateData();

            wb.Save("PivotTableFieldsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotFieldCollection](../../pivotfieldcollection/)
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


