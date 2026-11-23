---
title: "Cell.IsCheckBoxStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Indique si cette cellule est définie comme case à cocher"
type: docs
url: /fr/net/aspose.cells/cell/ischeckboxstyle/
---
## Cell.IsCheckBoxStyle property

Indique si la cellule est définie comme case à cocher.

```csharp
public bool IsCheckBoxStyle { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsCheckBoxStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accédez à la cellule B1 et définissez-la en style case à cocher
            Cell cell = worksheet.Cells["B1"];
            cell.IsCheckBoxStyle = true;
            cell.PutValue(true);
            
            // Accédez à la cellule A1 et définissez-la en style case à cocher avec une valeur
            cell = worksheet.Cells["A1"];
            cell.IsCheckBoxStyle = true;
            cell.PutValue(false);
            
            // Enregistrez le classeur
            workbook.Save("CheckBoxStyleDemo.xlsx");
            
            // Chargez le classeur enregistré pour vérifier les propriétés
            Workbook loadedWorkbook = new Workbook("CheckBoxStyleDemo.xlsx");
            worksheet = loadedWorkbook.Worksheets[0];
            
            // Vérifiez que B1 est en style case à cocher
            cell = worksheet.Cells["B1"];
            Console.WriteLine("Cell B1 IsCheckBoxStyle: " + cell.IsCheckBoxStyle);
            
            // Changez B1 en style non case à cocher et enregistrez
            cell.IsCheckBoxStyle = false;
            loadedWorkbook.Save("CheckBoxStyleDemo_Modified.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


