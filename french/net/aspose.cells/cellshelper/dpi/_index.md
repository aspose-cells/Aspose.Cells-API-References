---
title: "CellsHelper.DPI"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CellsHelper. Obtient le DPI de la machine"
type: docs
url: /fr/net/aspose.cells/cellshelper/dpi/
---
## CellsHelper.DPI property

Obtient le DPI de la machine.

```csharp
public static double DPI { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyDPIDemo
    {
        public static void Run()
        {
            // Définir et afficher le DPI actuel
            Console.WriteLine("Original DPI: " + CellsHelper.DPI);
            
            // Modifier le paramètre DPI
            CellsHelper.DPI = 300;
            Console.WriteLine("New DPI: " + CellsHelper.DPI);

            // Créer un nouveau classeur et enregistrer avec différents paramètres DPI
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajouter une forme d'exemple pour démontrer l'effet du DPI
            sheet.Shapes.AddRectangle(1, 1, 10, 10, 100, 100);

            // Enregistrer avec le paramètre DPI actuel
            workbook.Save("output_with_dpi_300.xlsx");

            // Modifier le DPI et enregistrer à nouveau
            CellsHelper.DPI = 96;
            workbook.Save("output_with_dpi_96.xlsx");
        }
    }
}
```

### Voir aussi

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


