---
title: "Classe Timeline"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Timelines.Timeline. Description résumée de la vue Timeline en raison du fait que MS Excel 2003 ne prend pas en charge Timeline"
type: docs
url: /fr/net/aspose.cells.timelines/timeline/
---
## Timeline class

Description résumée de la vue Chronologie En raison de MS Excel, Excel 2003 ne prend pas en charge la Chronologie.

```csharp
public class Timeline
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Caption](../../aspose.cells.timelines/timeline/caption/) { get; set; } | Obtient ou définit la légende de ce Timeline. |
| [CurrentLevel](../../aspose.cells.timelines/timeline/currentlevel/) { get; set; } | Le niveau de temps actuel du Timeline. |
| [HeightPixel](../../aspose.cells.timelines/timeline/heightpixel/) { get; set; } | (**Obsolete.**) Retourne ou définit la hauteur du timeline spécifié, en pixels. |
| [LeftPixel](../../aspose.cells.timelines/timeline/leftpixel/) { get; set; } | (**Obsolete.**) Retourne ou définit le décalage horizontal de la forme du timeline depuis sa colonne de gauche, en pixels. |
| [Name](../../aspose.cells.timelines/timeline/name/) { get; set; } | Retourne ou définit le nom du Timeline spécifié |
| [SelectionLevel](../../aspose.cells.timelines/timeline/selectionlevel/) { get; set; } | Obtient et définit le niveau de temps auquel la sélection actuelle a été faite pour le Timeline. |
| [Shape](../../aspose.cells.timelines/timeline/shape/) { get; } | Retourne l'objet [`TimelineShape`](../../aspose.cells.drawing/timelineshape/) associé à ce Timeline. |
| [ShowHeader](../../aspose.cells.timelines/timeline/showheader/) { get; set; } | Indique s'il faut afficher l'en-tête de ce timeline. |
| [ShowHorizontalScrollbar](../../aspose.cells.timelines/timeline/showhorizontalscrollbar/) { get; set; } | Indique s'il faut afficher la barre de défilement horizontale. |
| [ShowSelectionLabel](../../aspose.cells.timelines/timeline/showselectionlabel/) { get; set; } | Indique s'il faut afficher le libellé de sélection. |
| [ShowTimeLevel](../../aspose.cells.timelines/timeline/showtimelevel/) { get; set; } | Indique s'il faut afficher la boîte de sélection déroulante du niveau de temps. |
| [StartDate](../../aspose.cells.timelines/timeline/startdate/) { get; set; } | Obtient et définit la date de début de la position de défilement de la plage temporelle de ce `Timeline`. |
| [TopPixel](../../aspose.cells.timelines/timeline/toppixel/) { get; set; } | (**Obsolete.**) Renvoie ou définit le décalage vertical de la forme de la chronologie depuis sa rangée supérieure, en pixels. |
| [WidthPixel](../../aspose.cells.timelines/timeline/widthpixel/) { get; set; } | (**Obsolete.**) Renvoie ou définit la largeur de la chronologie spécifiée, en pixels. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetSelectedDateTimeRange](../../aspose.cells.timelines/timeline/getselecteddatetimerange/)() | Obtient la plage sélectionnée de date et heure. |
| [Select](../../aspose.cells.timelines/timeline/select/)(DateTime, DateTime, bool) | Sélectionne l'élément entre les dates et heures. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using Aspose.Cells.Timelines;
    using System;

    public class TimelineDemo
    {
        public static void TimelineExample()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Remplit la feuille de calcul avec des données d'exemple
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";

            // Créer un style de date
            Style dateStyle = new CellsFactory().CreateStyle();
            dateStyle.Custom = "m/d/yyyy";
            cells[0, 1].Value = "date";
            cells[1, 1].Value = new DateTime(2021, 2, 5);
            cells[2, 1].Value = new DateTime(2022, 3, 8);
            cells[3, 1].Value = new DateTime(2023, 4, 10);
            cells[4, 1].Value = new DateTime(2024, 5, 16);
            // Définir le style de date
            cells[1, 1].SetStyle(dateStyle);
            cells[2, 1].SetStyle(dateStyle);
            cells[3, 1].SetStyle(dateStyle);
            cells[4, 1].SetStyle(dateStyle);

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;

            // Ajouter un tableau croisé dynamique
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C5", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "date");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Actualiser les données du tableau croisé dynamique
            pivot.RefreshData();
            pivot.CalculateData();

            // Ajouter une nouvelle chronologie en utilisant le tableau croisé dynamique comme source de données
            sheet.Timelines.Add(pivot, 10, 5, "date");

            // Obtenir l'objet Timeline
            Timeline timelineObj = sheet.Timelines[0];

            // Définir les propriétés du Timeline
            timelineObj.Caption = "timeline caption test";
            timelineObj.Name = "timeline name test";
            timelineObj.LeftPixel = 100;
            timelineObj.TopPixel = 50;
            timelineObj.WidthPixel = 300;
            timelineObj.HeightPixel = 100;

            // Enregistrez le classeur
            book.Save("TimelineExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Timelines](../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../)


