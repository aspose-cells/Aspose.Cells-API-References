---
title: "Cells.GetRowEnumerator"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient l’énumérateur de lignes"
type: docs
url: /fr/net/aspose.cells/cells/getrowenumerator/
---
## Cells.GetRowEnumerator method

Obtient l’énumérateur de lignes.

```csharp
[Obsolete("Use RowCollection.GetEnumerator() method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetRowEnumerator()
```

### Valeur de retour

L’énumérateur de lignes.

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode RowCollection.GetEnumerator(). Cette méthode sera supprimée 12 mois après mai 2023. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsMethodGetRowEnumeratorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Row 1 Data");
            worksheet.Cells["A3"].PutValue("Row 3 Data");
            worksheet.Cells["A5"].PutValue("Row 5 Data");

            try
            {
                // Obtenez l’énumérateur de lignes à partir de la collection Cells
                IEnumerator enumerator = worksheet.Cells.GetRowEnumerator();
                
                Console.WriteLine("Iterating through rows containing data:");
                while (enumerator.MoveNext())
                {
                    Row row = (Row)enumerator.Current;
                    Cell cell = row.GetCellOrNull(0); // Get first cell in row
                    string cellValue = cell != null ? cell.Value.ToString() : "empty";
                    Console.WriteLine($"Row {row.Index}: First cell value = {cellValue}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRowEnumerator method: {ex.Message}");
            }
            
            // Enregistrez le classeur
            workbook.Save("MethodGetRowEnumeratorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* method [GetEnumerator](../../rowcollection/getenumerator/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


