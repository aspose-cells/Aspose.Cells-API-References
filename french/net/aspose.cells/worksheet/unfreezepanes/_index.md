---
title: "Worksheet.UnFreezePanes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Worksheet method. Débloque les volets dans la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/unfreezepanes/
---
## Worksheet.UnFreezePanes method

Défige les volets dans la feuille de calcul.

```csharp
public void UnFreezePanes()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodUnFreezePanesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Figer les volets à la cellule C3 (lignes 2, colonnes 2 figées)
            worksheet.FreezePanes("C3", 2, 2);

            // Vérifier que les volets sont figés
            int frozenRow, frozenColumn, frozenRows, frozenColumns;
            worksheet.GetFreezedPanes(out frozenRow, out frozenColumn, out frozenRows, out frozenColumns);
            Console.WriteLine($"Frozen panes - Row: {frozenRow}, Column: {frozenColumn}, Rows: {frozenRows}, Columns: {frozenColumns}");

            // Dégeler les volets
            worksheet.UnFreezePanes();

            // Vérifier que les volets sont défigés
            worksheet.GetFreezedPanes(out frozenRow, out frozenColumn, out frozenRows, out frozenColumns);
            Console.WriteLine($"After UnFreezePanes - Row: {frozenRow}, Column: {frozenColumn}, Rows: {frozenRows}, Columns: {frozenColumns}");

            // Enregistrez le classeur
            workbook.Save("UnFreezePanesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


