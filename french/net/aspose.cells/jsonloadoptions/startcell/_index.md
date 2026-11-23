---
title: "JsonLoadOptions.StartCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété JsonLoadOptions. Obtient et définit la cellule de départ"
type: docs
url: /fr/net/aspose.cells/jsonloadoptions/startcell/
---
## JsonLoadOptions.StartCell property

Obtient et définit la cellule de départ.

```csharp
public string StartCell { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsPropertyStartCellDemo
    {
        public static void Run()
        {
            // Créer des options de chargement JSON avec la propriété StartCell
            JsonLoadOptions options = new JsonLoadOptions
            {
                StartCell = "B3" // JSON data will start from cell B3
            };

            // Créer un classeur à partir d'un fichier JSON avec des options
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Header");
            
            // Créer un fichier JSON d'exemple
            System.IO.File.WriteAllText("data.json", "{\"Name\":\"John\",\"Age\":30,\"City\":\"New York\"}");
            
            // Charger les données JSON dans le classeur
            workbook = new Workbook("data.json", options);

            // Enregistrez le classeur
            workbook.Save("JsonStartCellDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


