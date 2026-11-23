---
title: "Énumération PivotTableAutoFormatType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Pivot.PivotTableAutoFormatType. Représente le type de formatage automatique du tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivottableautoformattype/
---
## PivotTableAutoFormatType enumeration

Représente le type de formatage automatique du tableau croisé dynamique.

```csharp
public enum PivotTableAutoFormatType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Représente le type de format Aucun. |
| Classic | `1` | Représente le type de format automatique Classique. |
| Report1 | `2` | Représente le type de format Report1. |
| Report2 | `3` | Représente le type de format Report2. |
| Report3 | `4` | Représente le type de format Report3. |
| Report4 | `5` | Représente le type de format Report4. |
| Report5 | `6` | Représente le type de format Report5. |
| Report6 | `7` | Représente le type de format Report6. |
| Report7 | `8` | Représente le type de format Report7. |
| Report8 | `9` | Représente le type de format Report8. |
| Report9 | `10` | Représente le type de format Report9. |
| Report10 | `11` | Représente le type de format Report10. |
| Table1 | `12` | Représente le type de format Table1. |
| Table2 | `13` | Représente le type de format Table2. |
| Table3 | `14` | Représente le type de format Table3. |
| Table4 | `15` | Représente le type de format Table4. |
| Table5 | `16` | Représente le type de format Table5. |
| Table6 | `17` | Représente le type de format Table6. |
| Table7 | `18` | Représente le type de format Table7. |
| Table8 | `19` | Représente le type de format Table8. |
| Table9 | `20` | Représente le type de format Table9. |
| Table10 | `21` | Représente le type de format Table10. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableAutoFormatTypeDemo
    {
        public static void PivotTableAutoFormatTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple pour le PivotTable
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 0].Value = "Apple";
            worksheet.Cells[3, 1].Value = 2021;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 0].Value = "Banana";
            worksheet.Cells[4, 1].Value = 2021;
            worksheet.Cells[4, 2].Value = 80;

            // Ajoutez un PivotTable à la feuille de calcul
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajoutez des champs au PivotTable
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Définissez le type de format automatique pour le PivotTable
            pivotTable.AutoFormatType = PivotTableAutoFormatType.Report1;

            // Enregistrez le classeur
            workbook.Save("PivotTableAutoFormatTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


