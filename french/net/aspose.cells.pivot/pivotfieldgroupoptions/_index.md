---
title: "Classe PivotFieldGroupOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Pivot.PivotFieldGroupOptions. Options pour les paramètres de regroupement du champ du tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfieldgroupoptions/
---
## PivotFieldGroupOptions class

Options pour les paramètres de regroupement du champ de tableau croisé dynamique.

```csharp
public class PivotFieldGroupOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PivotFieldGroupOptions](pivotfieldgroupoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [DiscreteGroupItems](../../aspose.cells.pivot/pivotfieldgroupoptions/discretegroupitems/) { get; set; } | Obtient et définit les éléments de groupe discrets. |
| [EndDate](../../aspose.cells.pivot/pivotfieldgroupoptions/enddate/) { get; set; } | Obtient ou définit la valeur de fin de la plage de regroupement. |
| [EndNumber](../../aspose.cells.pivot/pivotfieldgroupoptions/endnumber/) { get; set; } | Obtient ou définit la valeur de fin de la plage de regroupement. |
| [GroupType](../../aspose.cells.pivot/pivotfieldgroupoptions/grouptype/) { get; set; } | Obtient ou définit le type de regroupement pour le champ du tableau croisé dynamique. Seulement pour le champ de date/heure. |
| [GroupTypes](../../aspose.cells.pivot/pivotfieldgroupoptions/grouptypes/) { get; set; } | Obtient ou définit le type de regroupement pour le champ du tableau croisé dynamique. |
| [Interval](../../aspose.cells.pivot/pivotfieldgroupoptions/interval/) { get; set; } | Obtient ou définit la taille d’intervalle pour chaque groupe. |
| [IsAutoEnd](../../aspose.cells.pivot/pivotfieldgroupoptions/isautoend/) { get; set; } | Obtient ou définit une valeur indiquant si la valeur de fin est déterminée automatiquement. |
| [IsAutoStart](../../aspose.cells.pivot/pivotfieldgroupoptions/isautostart/) { get; set; } | Obtient ou définit une valeur indiquant si la valeur de départ est déterminée automatiquement. |
| [NewPivotField](../../aspose.cells.pivot/pivotfieldgroupoptions/newpivotfield/) { get; set; } | Obtient ou définit une valeur indiquant si de nouveaux champs du tableau croisé dynamique doivent être créés après le regroupement. |
| [StartDate](../../aspose.cells.pivot/pivotfieldgroupoptions/startdate/) { get; set; } | Obtient ou définit la valeur de départ de la plage de regroupement. |
| [StartNumber](../../aspose.cells.pivot/pivotfieldgroupoptions/startnumber/) { get; set; } | Obtient ou définit la valeur de départ de la plage de regroupement. |

### Exemples

```csharp

[C#]

// Charger le classeur d’exemple
Workbook wb = new Workbook("sampleGroupPivotFieldsInPivotTable.xlsx");
// Accéder à la deuxième feuille de calcul et à son tableau croisé dynamique
PivotTable pt = wb.Worksheets[1].PivotTables[0];
// Regrouper le premier champ de ligne (un champ de date) par mois et trimestres
PivotFieldGroupOptions options = new PivotFieldGroupOptions();
options.StartDate = new DateTime(2008, 1, 1);
options.EndDate = new DateTime(2008, 9, 5);
options.GroupTypes = new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Quarters };
pt.RowFields[0].Group(options);
// Calculer les données du tableau croisé dynamique et enregistrer le fichier de sortie
pt.CalculateData();
wb.Save("outputGroupPivotFieldsInPivotTable.xlsx");

[Visual Basic]

'Load the sample workbook
Dim wb As New Workbook("sampleGroupPivotFieldsInPivotTable.xlsx")
'Access the second worksheet and its pivot table
Dim pt As PivotTable = wb.Worksheets(1).PivotTables(0)
'Group the first row field (a date field) by months and quarters
Dim options As New PivotFieldGroupOptions()
options.StartDate = New DateTime(2008, 1, 1)
options.EndDate = New DateTime(2008, 9, 5)
options.GroupTypes = New PivotGroupByType() {PivotGroupByType.Months, PivotGroupByType.Quarters}
pt.RowFields(0).Group(options)
'Calculate the pivot table data and save the output file
pt.CalculateData()
wb.Save("outputGroupPivotFieldsInPivotTable.xlsx")
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


