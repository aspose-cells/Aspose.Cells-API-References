---
title: "Worksheet.GetFreezedPanes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Obtient les volets figés"
type: docs
url: /fr/net/aspose.cells/worksheet/getfreezedpanes/
---
## Worksheet.GetFreezedPanes method

Obtient les volets figés.

```csharp
public bool GetFreezedPanes(out int row, out int column, out int freezedRows, 
    out int freezedColumns)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32& | Index de ligne. |
| column | Int32& | Index de colonne. |
| freezedRows | Int32& | Nombre de lignes visibles dans le volet supérieur, ne dépassant pas l'index de ligne. |
| freezedColumns | Int32& | Nombre de colonnes visibles dans le volet gauche, ne dépassant pas l'index de colonne. |

### Valeur de retour

Retourne si la feuille de calcul est figée

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodGetFreezedPanesWithInt32ParametersDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Figer les volets à la cellule C5 (ligne 4, colonne 2) avec 2 lignes figées et 1 colonne figée
            worksheet.FreezePanes(4, 2, 2, 1);

            // Déclarer des variables pour stocker les informations des volets figés
            int row = 0;
            int column = 0;
            int freezedRows = 0;
            int freezedColumns = 0;

            try
            {
                // Appeler la méthode GetFreezedPanes avec des paramètres de sortie
                bool hasFreeze = worksheet.GetFreezedPanes(out row, out column, out freezedRows, out freezedColumns);

                // Affichez les résultats
                Console.WriteLine("Worksheet has freeze panes: " + hasFreeze);
                if (hasFreeze)
                {
                    Console.WriteLine("Freeze position - Row: " + row + ", Column: " + column);
                    Console.WriteLine("Frozen rows: " + freezedRows + ", Frozen columns: " + freezedColumns);
                }

                // Enregistrez le classeur
                workbook.Save("WorksheetMethodGetFreezedPanesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFreezedPanes method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


