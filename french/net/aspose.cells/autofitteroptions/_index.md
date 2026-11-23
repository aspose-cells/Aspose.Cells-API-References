---
title: "Classe AutoFitterOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.AutoFitterOptions. Représente toutes les options d'ajustement automatique"
type: docs
url: /fr/net/aspose.cells/autofitteroptions/
---
## AutoFitterOptions class

Représente toutes les options d'ajustement automatique.

```csharp
public class AutoFitterOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [AutoFitterOptions](autofitteroptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AutoFitMergedCells](../../aspose.cells/autofitteroptions/autofitmergedcells/) { get; set; } | (**Obsolete.**) Indique si la hauteur de ligne s'ajuste automatiquement lorsque les cellules sont fusionnées dans une ligne. La valeur par défaut est false. |
| [AutoFitMergedCellsType](../../aspose.cells/autofitteroptions/autofitmergedcellstype/) { get; set; } | Obtient et définit le type d'ajustement automatique de la hauteur de ligne des cellules fusionnées. |
| [AutoFitWrappedTextType](../../aspose.cells/autofitteroptions/autofitwrappedtexttype/) { get; set; } | Obtient et définit le type d'ajustement automatique du texte enveloppé. |
| [DefaultEditLanguage](../../aspose.cells/autofitteroptions/defaulteditlanguage/) { get; set; } | Obtient ou définit la langue d'édition par défaut. |
| [FormatStrategy](../../aspose.cells/autofitteroptions/formatstrategy/) { get; set; } | Obtient et définit la stratégie de formatage. |
| [ForRendering](../../aspose.cells/autofitteroptions/forrendering/) { get; set; } | Indique si l'ajustement est destiné au rendu. |
| [IgnoreHidden](../../aspose.cells/autofitteroptions/ignorehidden/) { get; set; } | Ignore les lignes/colonnes masquées. |
| [MaxRowHeight](../../aspose.cells/autofitteroptions/maxrowheight/) { get; set; } | Obtient et définit la hauteur maximale de ligne (en unité de Point) lors de l'ajustement automatique des lignes. |
| [OnlyAuto](../../aspose.cells/autofitteroptions/onlyauto/) { get; set; } | Indique si l'ajustement ne concerne que les lignes dont la hauteur n'est pas personnalisée. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitterOptionsDemo
    {
        public static void AutoFitterOptionsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("This is a sample text that will be wrapped and autofitted.");

            Style style = worksheet.Cells["A1"].GetStyle();

            style.IsTextWrapped = true;

            worksheet.Cells["A1"].SetStyle(style);

            // Créer une plage A1:B2
            Range range = worksheet.Cells.CreateRange(0, 0, 2, 2);

            // Fusionner les cellules
            range.Merge();

            // Créez une instance de AutoFitterOptions
            AutoFitterOptions options = new AutoFitterOptions
            {
                DefaultEditLanguage = DefaultEditLanguage.English,
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                OnlyAuto = true,
                IgnoreHidden = true,
                MaxRowHeight = 50.0,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                ForRendering = true
            };

            // Appliquez l'ajustement automatique des lignes avec les options spécifiées
            worksheet.AutoFitRows(options);

            // Enregistrez le classeur
            workbook.Save("AutoFitterOptionsExample.xlsx");
            workbook.Save("AutoFitterOptionsExample.pdf");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


