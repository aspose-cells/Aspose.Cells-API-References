---
title: "PivotField.Position"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Représente l'index de PivotField dans la région"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/position/
---
## PivotField.Position property

Représente l'index de [`PivotField`](../) dans la région.

```csharp
public int Position { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyPositionDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook wb = new Workbook("NET46429_a.xlsx");
            
            // Accédez à la première feuille de calcul et à son tableau croisé dynamique
            Worksheet ws = wb.Worksheets[0];
            PivotTable pt = ws.PivotTables[0];
            
            // Démontrez l'utilisation de la propriété Position
            int position = pt.PageFields[0].Position;
            Console.WriteLine("Position of first page field: " + position);
            
            // Utilisez la position pour afficher les pages de filtre de rapport
            pt.ShowReportFilterPageByIndex(position);
            
            // Enregistrez le classeur
            wb.Save("PivotFieldPropertyPositionDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


