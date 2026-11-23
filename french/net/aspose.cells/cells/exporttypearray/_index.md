---
title: "Cells.ExportTypeArray"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Exporte le type de valeur des cellules de la collection Cells vers un objet tableau à deux dimensions"
type: docs
url: /fr/net/aspose.cells/cells/exporttypearray/
---
## Cells.ExportTypeArray method

Exporte le type de valeur des cellules de la collection [`Cells`](../) vers un objet tableau à deux dimensions.

```csharp
public CellValueType[] ExportTypeArray(int firstRow, int firstColumn, int totalRows, 
    int totalColumns)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | Le numéro de ligne de la première cellule à exporter. |
| firstColumn | Int32 | Le numéro de colonne de la première cellule à exporter. |
| totalRows | Int32 | Nombre de lignes à exporter. |
| totalColumns | Int32 | Nombre de colonnes à exporter. |

### Valeur de retour

Objet tableau exporté représentant les types de valeurs des cellules.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportTypeArrayWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir les valeurs dans les cellules
            cells["A1"].PutValue(10);
            cells["B1"].PutValue("Hello");
            cells["A2"].PutValue(true);
            cells["B2"].PutValue(DateTime.Now);

            // Exporter les types de cellules vers un tableau 2D
            CellValueType[,] typeArray = cells.ExportTypeArray(0, 0, 2, 2);

            // Affichez les résultats
            for (int i = 0; i < 2; i++)
            {
                for (int j = 0; j < 2; j++)
                {
                    Console.WriteLine($"Cell[{i},{j}] Type: {typeArray[i, j]}");
                }
            }

            // Démontrer le cas d'exception
            try
            {
                CellValueType[,] invalidArray = cells.ExportTypeArray(-1, 0, 2, 2);
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Exception caught as expected: " + ex.Message);
            }
        }
    }
}
```

### Voir aussi

* enum [CellValueType](../../cellvaluetype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


