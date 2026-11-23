---
title: "Classe PivotFieldTop10AutoShowSettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Pivot.PivotFieldTop10AutoShowSettings. Représente les paramètres Top 10 AutoShow pour un champ pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfieldtop10autoshowsettings/
---
## PivotFieldTop10AutoShowSettings class

Représente les paramètres Top 10 AutoShow pour un champ de tableau croisé dynamique.

```csharp
public class PivotFieldTop10AutoShowSettings
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AutoShowCount](../../aspose.cells.pivot/pivotfieldtop10autoshowsettings/autoshowcount/) { get; set; } | Représente le nombre d'éléments supérieurs ou inférieurs affichés automatiquement dans le champ PivotTable spécifié. |
| [IsAutoShow](../../aspose.cells.pivot/pivotfieldtop10autoshowsettings/isautoshow/) { get; set; } | Indique si un filtre "Top 10 AutoShow" est appliqué à ce champ. |
| [IsTop](../../aspose.cells.pivot/pivotfieldtop10autoshowsettings/istop/) { get; set; } | Indique si le champ de tableau croisé dynamique spécifié est affiché automatiquement en ordre croissant. |
| [RankBy](../../aspose.cells.pivot/pivotfieldtop10autoshowsettings/rankby/) { get; set; } | Spécifie l'index du champ de données pour le classement AutoShow. Représente l'index du champ affiché automatiquement. -1 signifie le PivotField lui‑même. Il doit s'agir de l'index des champs de données. |

### Remarques

Dans xls : mise en œuvre des filtres Top 10 dans Xls via Top 10 AutoShow. Dans les fichiers ooxml : le format de fichier ooxml sous‑jacent prend en charge Top10 AutoShow, mais l'interface utilisateur d'Excel 2007 et versions ultérieures n'offre l'accès que via le filtre Top10. Si la compatibilité XLS n'est pas requise, il est recommandé d'utiliser le filtre Top10 à la place.

### Exemples

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

PivotTable pivot = pivots.Add("=Sheet1!A1:C9", "A12");

pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");
           
pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
           
 //Modifier les attributs du PivotField
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

//Afficher les 2 premiers éléments par libellé de champ de ligne.
rowField.Top10AutoShow(true, true, 2, -1);

PivotFieldTop10AutoShowSettings sortSetting = rowField.Top10AutoShowSettings;
Console.WriteLine(sortSetting.IsAutoShow);

 pivot.CalculateData();

book.Save("out.xlsx");

[Visual Basic]

Dim book As New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells
cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables

Dim pivot As PivotTable = pivots.Add("=Sheet1!A1:C9", "A12")
 
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
pivot.AddFieldToArea(PivotFieldType.Column, "year")
pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

'Show top 2 items by row field label.
rowField.Top10AutoShow(True, True, 2, -1)

Dim sortSetting As PivotFieldTop10AutoShowSettings = rowField.Top10AutoShowSettings
Console.WriteLine(sortSetting.IsAutoShow)

pivot.CalculateData()

book.Save("out.xlsx")
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


