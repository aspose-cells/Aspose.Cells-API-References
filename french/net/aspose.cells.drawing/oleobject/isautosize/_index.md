---
title: "OleObject.IsAutoSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OleObject. True indique que la taille de l'objet ole sera automatiquement modifiée en fonction de la taille de l'instantané du contenu incorporé lorsque l'objet ole est activé"
type: docs
url: /fr/net/aspose.cells.drawing/oleobject/isautosize/
---
## OleObject.IsAutoSize property

Vrai indique que la taille de l'objet OLE sera automatiquement modifiée en fonction de la taille de l'instantané du contenu intégré lorsque l'objet OLE est activé.

```csharp
public bool IsAutoSize { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un objet OLE (en utilisant les données du fichier sous forme de tableau d'octets)
            byte[] oleData = System.IO.File.ReadAllBytes(@"C:\example\test.docx");
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, oleData);
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleIndex];

            // Définir et démontrer la propriété IsAutoSize
            oleObject.IsAutoSize = true;
            Console.WriteLine("OLE Object AutoSize initially: " + oleObject.IsAutoSize);

            // Modifier la propriété
            oleObject.IsAutoSize = false;
            Console.WriteLine("OLE Object AutoSize after change: " + oleObject.IsAutoSize);

            // Enregistrez le classeur
            workbook.Save("OleObjectIsAutoSizeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


