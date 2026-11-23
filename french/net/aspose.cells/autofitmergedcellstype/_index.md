---
title: "Énumération AutoFitMergedCellsType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.AutoFitMergedCellsType enum. Représente le type d'ajustement automatique des cellules fusionnées"
type: docs
url: /fr/net/aspose.cells/autofitmergedcellstype/
---
## AutoFitMergedCellsType enumeration

Représente le type d'ajustement automatique des cellules fusionnées.

```csharp
public enum AutoFitMergedCellsType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Ignorer les cellules fusionnées. |
| FirstLine | `1` | N'augmente que la hauteur de la première ligne. |
| LastLine | `2` | N'augmente que la hauteur de la dernière ligne. |
| EachLine | `3` | Augmente la hauteur de chaque ligne. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitMergedCellsTypeDemo
    {
        public static void AutoFitMergedCellsTypeExample()
        {
            //Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            //Obtention de la référence de la feuille de calcul nouvellement ajoutée
            Worksheet sheet1 = workbook.Worksheets[0];

            // Créer une plage A1:B2
            Range range = sheet1.Cells.CreateRange(0, 0, 2, 2);

            // Fusionner les cellules
            range.Merge();

            // Insérer une valeur dans la cellule fusionnée A1
            sheet1.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Créez un objet de style
            Style style = sheet1.Cells[0, 0].GetStyle();

            // Activer le texte à la ligne
            style.IsTextWrapped = true;

            // Appliquez le style à la cellule
            sheet1.Cells[0, 0].SetStyle(style);

            // Créer un objet pour AutoFitterOptions
            AutoFitterOptions options = new AutoFitterOptions();

            // N'augmente que la hauteur de la première ligne.
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.FirstLine;

            // Ajuster automatiquement les lignes de la feuille (y compris les cellules fusionnées)
            sheet1.AutoFitRows(options);


            int index = workbook.Worksheets.Add();
            Worksheet sheet2 = workbook.Worksheets[index];
            sheet2.Name = "Sheet2";
            // Créer une plage A1:B2
            Range range2 = sheet2.Cells.CreateRange(0, 0, 2, 2);

            // Fusionner les cellules
            range2.Merge();

            // Insérer une valeur dans la cellule fusionnée A1
            sheet2.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Créez un objet de style
            Style style2 = sheet2.Cells[0, 0].GetStyle();

            // Activer le texte à la ligne
            style2.IsTextWrapped = true;

            // Appliquez le style à la cellule
            sheet2.Cells[0, 0].SetStyle(style);

            // Créer un objet pour AutoFitterOptions
            AutoFitterOptions options2 = new AutoFitterOptions();

            // N'augmente que la hauteur de la dernière ligne.
            options2.AutoFitMergedCellsType = AutoFitMergedCellsType.LastLine;

            // Ajuster automatiquement les lignes de la feuille (y compris les cellules fusionnées)
            sheet2.AutoFitRows(options2);


            index = workbook.Worksheets.Add();
            Worksheet sheet3 = workbook.Worksheets[index];
            sheet3.Name = "Sheet3";
            // Créer une plage A1:B2
            Range range3 = sheet3.Cells.CreateRange(0, 0, 2, 2);

            // Fusionner les cellules
            range3.Merge();

            // Insérer une valeur dans la cellule fusionnée A1
            sheet3.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Créez un objet de style
            Style style3 = sheet3.Cells[0, 0].GetStyle();

            // Activer le texte à la ligne
            style3.IsTextWrapped = true;

            // Appliquez le style à la cellule
            sheet3.Cells[0, 0].SetStyle(style);

            // Créer un objet pour AutoFitterOptions
            AutoFitterOptions options3 = new AutoFitterOptions();

            // N'augmente que la hauteur de chaque ligne.
            options3.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;

            // Ajuster automatiquement les lignes de la feuille (y compris les cellules fusionnées)
            sheet3.AutoFitRows(options3);


            index = workbook.Worksheets.Add();
            Worksheet sheet4 = workbook.Worksheets[index];
            sheet4.Name = "Sheet4";
            // Créer une plage A1:B2
            Range range4 = sheet4.Cells.CreateRange(0, 0, 2, 2);

            // Fusionner les cellules
            range4.Merge();

            // Insérer une valeur dans la cellule fusionnée A1
            sheet4.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Créez un objet de style
            Style style4 = sheet4.Cells[0, 0].GetStyle();

            // Activer le texte à la ligne
            style4.IsTextWrapped = true;

            // Appliquez le style à la cellule
            sheet4.Cells[0, 0].SetStyle(style);

            // Créer un objet pour AutoFitterOptions
            AutoFitterOptions options4 = new AutoFitterOptions();

            // Ignorer les cellules fusionnées.
            options4.AutoFitMergedCellsType = AutoFitMergedCellsType.None;

            // Ajuster automatiquement les lignes de la feuille (sans les cellules fusionnées)
            sheet4.AutoFitRows(options4);

            // Enregistrez le classeur
            workbook.Save("AutoFitMergedCellsTypeExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


