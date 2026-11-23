---
title: "HorizontalPageBreak.Row"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HorizontalPageBreak. Obtient l'index de ligne basé sur zéro"
type: docs
url: /fr/net/aspose.cells/horizontalpagebreak/row/
---
## HorizontalPageBreak.Row property

Obtient l'indice de ligne basé à zéro.

```csharp
public int Row { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakPropertyRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des ruptures de page horizontales
            worksheet.HorizontalPageBreaks.Add(6);
            worksheet.HorizontalPageBreaks.Add(12);

            // Obtenez la collection des ruptures de page horizontales
            HorizontalPageBreakCollection breaks = worksheet.HorizontalPageBreaks;

            // Affichez les numéros de ligne des ruptures de page
            Console.WriteLine("Page break at row: " + breaks[0].Row);
            Console.WriteLine("Page break at row: " + breaks[1].Row);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


