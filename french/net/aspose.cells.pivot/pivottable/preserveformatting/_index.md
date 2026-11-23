---
title: "PivotTable.PreserveFormatting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Indique si le formatage des cellules PivotTableFormat est conservé lorsque le PivotTable est actualisé ou recalculé"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/preserveformatting/
---
## PivotTable.PreserveFormatting property

Indique si le formatage des cellules ([`PivotTableFormat`](../../pivottableformat/)) est conservé lorsque le PivotTable est actualisé ou recalculé.

```csharp
[Obsolete("Use PivotTable.PreserveCellFormattingOnUpdate property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool PreserveFormatting { get; set; }
```

### Remarques

REMARQUE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotTable.PreserveCellFormattingOnUpdate. Cette méthode sera supprimée 12 mois après juillet 2026. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPreserveFormattingDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("source.xlsx");
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder au premier tableau croisé dynamique
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Activer la conservation du formatage lors de l’actualisation
            pivotTable.PreserveFormatting = true;
            
            // Appliquer un certain formatage à la zone de données du tableau croisé dynamique
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 10;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            // Formater la zone de données du tableau croisé dynamique
            pivotTable.FormatAll(style);
            
            // Actualiser et calculer les données du tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


