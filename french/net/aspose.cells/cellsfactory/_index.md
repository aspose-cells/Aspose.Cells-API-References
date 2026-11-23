---
title: "Classe CellsFactory"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.CellsFactory classe. Utilitaire pour instancier les classes du modèle Cells"
type: docs
url: /fr/net/aspose.cells/cellsfactory/
---
## CellsFactory class

Utilitaire pour instancier des classes du modèle Cells.

```csharp
public class CellsFactory
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [CellsFactory](cellsfactory/)() | Le constructeur par défaut. |

## Méthodes

| Nom | Description |
| --- | --- |
| [CreateStyle](../../aspose.cells/cellsfactory/createstyle/)() | Crée un nouveau style. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsFactoryDemo
    {
        public static void CellsFactoryExample()
        {
            // Créer une nouvelle instance de CellsFactory
            CellsFactory factory = new CellsFactory();

            // Utiliser la fabrique pour créer un nouveau Style
            Style style = factory.CreateStyle();

            // Personnaliser le style
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;

            // Créer un nouveau classeur et une nouvelle feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Appliquer le style à une cellule spécifique
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Styled Cell");
            cell.SetStyle(style);

            // Enregistrer le classeur dans un fichier
            workbook.Save("CellsFactoryExample.xlsx");
            workbook.Save("CellsFactoryExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


