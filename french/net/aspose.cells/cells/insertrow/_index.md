---
title: "Cells.InsertRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Insère une nouvelle ligne dans la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/cells/insertrow/
---
## Cells.InsertRow method

Insère une nouvelle ligne dans la feuille de calcul.

```csharp
public void InsertRow(int rowIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index de ligne. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet sheet = workbook.Worksheets[0];
            
            // Obtenir la collection de cellules
            Cells cells = sheet.Cells;
            
            // Insérez des données d'exemple dans la ligne 6
            cells[6, 0].PutValue("Original Row 6");
            cells[6, 1].PutValue(100);
            
            // Insérez des données d'exemple dans la ligne 7
            cells[7, 0].PutValue("Original Row 7");
            cells[7, 1].PutValue(200);
            
            // Insérez une nouvelle ligne à l'index 7 (déplace la ligne 7 existante vers le bas)
            cells.InsertRow(7);
            
            // Ajoutez des données à la ligne nouvellement insérée
            cells[7, 0].PutValue("New Inserted Row");
            cells[7, 1].PutValue(150);
            
            // Enregistrez le classeur
            workbook.Save("InsertRowDemo.xlsx");
            
            Console.WriteLine("Row inserted successfully at index 7.");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


