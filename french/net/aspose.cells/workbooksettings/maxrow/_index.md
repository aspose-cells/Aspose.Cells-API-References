---
title: "WorkbookSettings.MaxRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient l'index maximal de ligne basé sur zéro"
type: docs
url: /fr/net/aspose.cells/workbooksettings/maxrow/
---
## WorkbookSettings.MaxRow property

Obtient l'index maximal de ligne, basé sur zéro.

```csharp
public int MaxRow { get; }
```

### Remarques

Renvoie 65535 si le format de fichier est Excel97-2003;

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMaxRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Démontrer la propriété MaxRow
            Console.WriteLine("Maximum rows in worksheet: " + workbook.Settings.MaxRow);
            
            // Essayer d'accéder à une cellule au-delà de MaxRow (devrait lever une exception)
            try
            {
                Cell cell = worksheet.Cells[workbook.Settings.MaxRow + 1, 0];
                Console.WriteLine("This line shouldn't execute");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Expected error when accessing beyond MaxRow: " + ex.Message);
            }
            
            // Créer une zone de cellules en utilisant MaxRow
            CellArea area = CellArea.CreateCellArea(0, 0, workbook.Settings.MaxRow, 0);
            Console.WriteLine("Created cell area from row 0 to MaxRow: " + area.EndRow);
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


