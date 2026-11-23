---
title: "Cells.ExportArray"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Exporte les données de la collection Cells vers un objet tableau à deux dimensions"
type: docs
url: /fr/net/aspose.cells/cells/exportarray/
---
## Cells.ExportArray method

Exporte les données de la collection [`Cells`](../) vers un objet tableau à deux dimensions.

```csharp
public object[] ExportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | Le numéro de ligne de la première cellule à exporter. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule à exporter. |
| totalRows | Int32 | Nombre de lignes à exporter |
| totalColumns | Int32 | Nombre de colonnes à exporter |

### Valeur de retour

Objet tableau de valeurs de cellules exportées.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportArrayWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Remplir des données d'exemple
            cells[0, 0].PutValue("A");
            cells[0, 1].PutValue("B");
            cells[1, 0].PutValue(10);
            cells[1, 1].PutValue(20);

            try
            {
                // Exporter les données vers un tableau
                object[,] dataArray = cells.ExportArray(0, 0, 2, 2);
                
                // Afficher le tableau exporté
                for (int i = 0; i < 2; i++)
                {
                    for (int j = 0; j < 2; j++)
                    {
                        Console.Write(dataArray[i, j] + "\t");
                    }
                    Console.WriteLine();
                }
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Error exporting array: " + ex.Message);
            }
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


