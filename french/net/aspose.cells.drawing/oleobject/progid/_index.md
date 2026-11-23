---
title: "OleObject.ProgID"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OleObject. Obtient ou définit le ProgID de l'objet OLE"
type: docs
url: /fr/net/aspose.cells.drawing/oleobject/progid/
---
## OleObject.ProgID property

Obtient ou définit le ProgID de l'objet OLE.

```csharp
public string ProgID { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyProgIDDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un objet OLE à la feuille de calcul
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0], "test.pdf");
            OleObject ole = worksheet.OleObjects[oleIndex];
            
            // Définir le ProgID pour l'objet OLE
            ole.ProgID = "AcroExch.Document.DC";
            
            // Afficher le ProgID
            Console.WriteLine("OLE Object ProgID: " + ole.ProgID);

            // Enregistrez le classeur
            workbook.Save("OleObjectProgIDDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


