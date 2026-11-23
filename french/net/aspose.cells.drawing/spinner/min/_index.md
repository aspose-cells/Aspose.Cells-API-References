---
title: "Spinner.Min"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Spinner. Obtient ou définit la valeur minimale d'une barre de défilement ou d'une plage de spinner"
type: docs
url: /fr/net/aspose.cells.drawing/spinner/min/
---
## Spinner.Min property

Obtient ou définit la valeur minimale de la plage d'une barre de défilement ou d'un sélecteur

```csharp
public int Min { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyMinDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle de spinner avec les dimensions appropriées
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 1, 1, 1, 100, 20);

            // Définir les propriétés du spinner, y compris Min
            spinner.Min = 10;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 15;

            // Vérifier et afficher la propriété Min
            Console.WriteLine("Spinner Min Value: " + spinner.Min);

            // Enregistrez le classeur
            workbook.Save("SpinnerPropertyMinDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


