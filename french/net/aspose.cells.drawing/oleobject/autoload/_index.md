---
title: "OleObject.AutoLoad"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OleObject. Spécifie si l'application hôte de l'objet intégré doit être appelée pour charger les données de l'objet automatiquement lorsque le classeur parent est ouvert"
type: docs
url: /fr/net/aspose.cells.drawing/oleobject/autoload/
---
## OleObject.AutoLoad property

Spécifie si l'application hôte de l'objet intégré doit être appelée pour charger les données de l'objet automatiquement lorsque le classeur parent est ouvert.

```csharp
public bool AutoLoad { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyAutoLoadDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter un OleObject à la feuille de calcul
            int oleNumber = sheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            
            // Définir les propriétés OleObject
            OleObject ole = sheet.OleObjects[oleNumber];
            ole.ProgID = "Excel.Sheet";
            ole.ObjectData = new byte[0];
            
            // Démontrer la propriété AutoLoad
            ole.AutoLoad = true; // Automatically load the OleObject when the workbook opens
            
            // Enregistrez le classeur
            workbook.Save("OleObjectAutoLoadDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


