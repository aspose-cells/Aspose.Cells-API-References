---
title: "Cell.IsInTable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Indique si cette cellule fait partie d'une formule de tableau"
type: docs
url: /fr/net/aspose.cells/cell/isintable/
---
## Cell.IsInTable property

Indique si cette cellule fait partie d'une formule de tableau.

```csharp
[Obsolete("Use IsTableFormula instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsInTable { get; }
```

### Remarques

NOTE : Cette classe est maintenant obsolète. À la place, veuillez utiliser Cell.IsTableFormula pour vérifier si la formule de la cellule fait partie d'une formule de tableau. Cette propriété sera supprimée 12 mois plus tard à compter de mai 2018. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class CellPropertyIsInTableDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1.5);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(0.8);

            // Créer un tableau à partir de la plage de données
            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            try
            {
                // Vérifier la propriété IsInTable pour les cellules à l'intérieur et à l'extérieur du tableau
                Cell cellInTable = worksheet.Cells["A2"];
                Cell cellOutsideTable = worksheet.Cells["C2"];

                Console.WriteLine("Cell A2 (inside table):");
                Console.WriteLine("  Value: " + cellInTable.StringValue);
                Console.WriteLine("  IsInTable: " + cellInTable.IsInTable);

                Console.WriteLine("\nCell C2 (outside table):");
                Console.WriteLine("  Value: " + cellOutsideTable.StringValue);
                Console.WriteLine("  IsInTable: " + cellOutsideTable.IsInTable);

                // Enregistrez le classeur
                workbook.Save("IsInTableDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


