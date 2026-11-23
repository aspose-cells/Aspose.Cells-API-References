---
title: "WorkbookSettings.MaxRowsOfSharedFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient et définit le nombre maximal de lignes de la formule partagée"
type: docs
url: /fr/net/aspose.cells/workbooksettings/maxrowsofsharedformula/
---
## WorkbookSettings.MaxRowsOfSharedFormula property

Obtient et définit le numéro maximal de ligne de la formule partagée.

```csharp
public int MaxRowsOfSharedFormula { get; set; }
```

### Remarques

Si le nombre est trop grand, l'autofilter fonctionne très lentement dans MS Excel 2013.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMaxRowsOfSharedFormulaDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            book.Settings.MaxRowsOfSharedFormula = 100;
            
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Définir la formule partagée avec 101 lignes (dépassant MaxRowsOfSharedFormula)
            cells["B1"].SetSharedFormula("=A1", 101, 1);
            
            // Vérifier la formule dans la dernière cellule
            Console.WriteLine("Formula in B101: " + cells["B101"].Formula);
            
            // Augmenter MaxRowsOfSharedFormula et tester à nouveau dans une nouvelle feuille
            book.Settings.MaxRowsOfSharedFormula = 1024;
            Worksheet sheet2 = book.Worksheets.Add("Sheet2");
            cells = sheet2.Cells;
            cells["B1"].SetSharedFormula("=A1", 101, 1);
            
            Console.WriteLine("Formula in B101 (Sheet2): " + cells["B101"].Formula);
            
            book.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


