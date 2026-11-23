---
title: "Cells.GetFirstDataRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient l'index de la première ligne de la cellule qui contient des données dans la colonne spécifiée"
type: docs
url: /fr/net/aspose.cells/cells/getfirstdatarow/
---
## Cells.GetFirstDataRow method

Obtient l'index de la première ligne de la cellule qui contient des données dans la colonne spécifiée.

```csharp
public int GetFirstDataRow(int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| column | Int32 | Index de colonne. |

### Valeur de retour

index de la première ligne.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetFirstDataRowWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple pour démontrer la méthode
            worksheet.Cells["A1"].Value = "Header";
            worksheet.Cells["A2"].Value = "Data1";
            worksheet.Cells["A3"].Value = "Data2";
            worksheet.Cells["B5"].Value = "Data3";
            worksheet.Cells["C7"].Value = "Data4";

            try
            {
                // Obtenez la collection Cells de la feuille de calcul
                Cells cells = worksheet.Cells;

                // Appelez GetFirstDataRow pour la colonne A (index 0)
                int firstDataRowA = cells.GetFirstDataRow(0);
                Console.WriteLine($"First data row in column A: {firstDataRowA}");

                // Appelez GetFirstDataRow pour la colonne B (index 1)
                int firstDataRowB = cells.GetFirstDataRow(1);
                Console.WriteLine($"First data row in column B: {firstDataRowB}");

                // Appelez GetFirstDataRow pour la colonne C (index 2)
                int firstDataRowC = cells.GetFirstDataRow(2);
                Console.WriteLine($"First data row in column C: {firstDataRowC}");

                // Enregistrez le classeur
                workbook.Save("GetFirstDataRowDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


