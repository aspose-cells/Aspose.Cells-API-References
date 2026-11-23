---
title: "Worksheet.Zoom"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Représente le facteur d'échelle en pourcentage. Il doit être compris entre 10 et 400."
type: docs
url: /fr/net/aspose.cells/worksheet/zoom/
---
## Worksheet.Zoom property

Représente le facteur d'échelle en pourcentage. Il doit être compris entre 10 et 400.

```csharp
public int Zoom { get; set; }
```

### Remarques

Veuillez d'abord définir le type de vue.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyZoomDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir le facteur de zoom à 120 %
            worksheet.Zoom = 120;
            
            // Afficher le facteur de zoom actuel
            Console.WriteLine("Current worksheet zoom: " + worksheet.Zoom + "%");
            
            // Enregistrez le classeur
            workbook.Save("WorksheetZoomDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


