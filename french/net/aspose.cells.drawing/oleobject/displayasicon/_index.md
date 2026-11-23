---
title: "OleObject.DisplayAsIcon"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OleObject. Vrai si l'objet spécifié est affiché sous forme d'icône et que l'image ne sera pas modifiée automatiquement"
type: docs
url: /fr/net/aspose.cells.drawing/oleobject/displayasicon/
---
## OleObject.DisplayAsIcon property

Vrai si l'objet spécifié est affiché sous forme d'icône et que l'image ne sera pas modifiée automatiquement.

```csharp
public bool DisplayAsIcon { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyDisplayAsIconDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un objet OLE (PDF) à la feuille de calcul
            byte[] pdfData = File.ReadAllBytes("example.pdf");
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, pdfData);
            
            // Obtenir l'objet OLE
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleIndex];
            oleObject.ProgID = "AcroExch.Document.DC";
            
            // Démontrer la propriété DisplayAsIcon
            oleObject.DisplayAsIcon = true; // Show as icon
            // oleObject.DisplayAsIcon = false; // Afficher le contenu si possible
            
            // Enregistrez le classeur
            workbook.Save("OleObjectDisplayAsIconDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


