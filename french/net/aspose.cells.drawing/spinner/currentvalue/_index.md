---
title: "Spinner.CurrentValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Spinner. Obtient ou définit la valeur actuelle"
type: docs
url: /fr/net/aspose.cells.drawing/spinner/currentvalue/
---
## Spinner.CurrentValue property

Obtient ou définit la valeur actuelle.

```csharp
public int CurrentValue { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyCurrentValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle de spinner
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Spinner, 1, 1, 0, 0, 20, 20);
            Spinner spinner = (Spinner)shape;

            // Définir les propriétés du Spinner
            spinner.LinkedCell = "A1";
            spinner.Min = 1;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 10; // Using CurrentValue property directly

            // Vérifier et afficher la valeur actuelle
            Console.WriteLine("Spinner CurrentValue: " + spinner.CurrentValue);

            // Enregistrez le classeur
            workbook.Save("SpinnerDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


