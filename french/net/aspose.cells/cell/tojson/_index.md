---
title: "Cell.ToJson"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Convertir Cell en données de structure JSON"
type: docs
url: /fr/net/aspose.cells/cell/tojson/
---
## Cell.ToJson method

Convertir [`Cell`](../) en données de structure JSON.

```csharp
public string ToJson()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodToJsonDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir des données d'exemple et des styles
            cells["A1"].PutValue(100);
            cells["B6"].Formula = "=A1";
            
            // Obtenir la cellule et convertir en JSON
            Cell cell = cells["B6"];
            string json = cell.ToJson();
            
            // Générez le JSON
            Console.WriteLine("Cell JSON:");
            Console.WriteLine(json);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


