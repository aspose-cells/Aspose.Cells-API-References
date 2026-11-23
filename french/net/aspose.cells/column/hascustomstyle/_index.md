---
title: "Column.HasCustomStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Column. Indique si cette colonne possède des paramètres de style personnalisés différents du style par défaut hérité du classeur"
type: docs
url: /fr/net/aspose.cells/column/hascustomstyle/
---
## Column.HasCustomStyle property

Indique si cette colonne possède des paramètres de style personnalisés (différents du paramètre par défaut hérité du classeur).

```csharp
public bool HasCustomStyle { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la première colonne
            Column column = worksheet.Cells.Columns[0];

            // Afficher la valeur initiale de HasCustomState
            Console.WriteLine("Initial HasCustomStyle: " + column.HasCustomStyle);

            // Modifier le style de la colonne pour démontrer le changement de HasCustomStyle
            Style columnStyle = column.GetStyle();
            columnStyle.BackgroundColor = Color.LightBlue;
            column.SetStyle(columnStyle);

            // Afficher la valeur mise à jour de HasCustomStyle
            Console.WriteLine("After style modification - HasCustomStyle: " + column.HasCustomStyle);

            // Créer une autre colonne avec le style par défaut pour la comparaison
            Column secondColumn = worksheet.Cells.Columns[1];
            Console.WriteLine("Second column HasCustomStyle: " + secondColumn.HasCustomStyle);

            // Enregistrez le classeur
            workbook.Save("ColumnHasCustomStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


