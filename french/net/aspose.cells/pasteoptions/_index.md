---
title: "Classe PasteOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.PasteOptions. Représente les options de collage spécial"
type: docs
url: /fr/net/aspose.cells/pasteoptions/
---
## PasteOptions class

Représente les options de collage spécial.

```csharp
public class PasteOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PasteOptions](pasteoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [IgnoreLinksToOriginalFile](../../aspose.cells/pasteoptions/ignorelinkstooriginalfile/) { get; set; } | Ignorer les liens vers le fichier original. |
| [KeepOldTables](../../aspose.cells/pasteoptions/keepoldtables/) { get; set; } | Conserve les tableaux dans la plage de destination. |
| [OnlyVisibleCells](../../aspose.cells/pasteoptions/onlyvisiblecells/) { get; set; } | Vrai signifie ne copier que les cellules visibles. |
| [OperationType](../../aspose.cells/pasteoptions/operationtype/) { get; set; } | Obtient et définit le type d'opération lors du collage de la plage. |
| [PasteType](../../aspose.cells/pasteoptions/pastetype/) { get; set; } | Le type de collage spécial. |
| [ShiftFormulasOfShapes](../../aspose.cells/pasteoptions/shiftformulasofshapes/) { get; set; } | Indique s'il faut décaler les formules des formes lors de la copie des plages. |
| [SkipBlanks](../../aspose.cells/pasteoptions/skipblanks/) { get; set; } | Indique s'il faut ignorer les cellules vides. |
| [Transpose](../../aspose.cells/pasteoptions/transpose/) { get; set; } | Vrai pour transposer les lignes et les colonnes lorsque la plage est collée. La valeur par défaut est Faux. |

### Exemples

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsDemo
    {
        public static void PasteOptionsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données à la première feuille de calcul
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");
            sheet.Cells["A3"].PutValue(123);

            // Créez une autre feuille de calcul
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");

            // Définir la plage source
            Aspose.Cells.Range sourceRange = sheet.Cells.CreateRange("A1:A3");

            // Définir la plage de destination
            Aspose.Cells.Range destRange = sheet2.Cells.CreateRange("B1:B3");

            // Créez l'objet PasteOptions
            PasteOptions pasteOptions = new PasteOptions
            {
                PasteType = PasteType.Values,
                SkipBlanks = true,
                OnlyVisibleCells = false,
                Transpose = false,
                OperationType = PasteOperationType.None,
                IgnoreLinksToOriginalFile = true
            };

            // Copiez la plage avec les options de collage spécifiées
            destRange.Copy(sourceRange, pasteOptions);

            // Enregistrez le classeur
            workbook.Save("PasteOptionsExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


