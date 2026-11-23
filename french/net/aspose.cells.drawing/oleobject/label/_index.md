---
title: "OleObject.Label"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OleObject. Obtient et définit le libellé d'affichage de l'objet ole lié"
type: docs
url: /fr/net/aspose.cells.drawing/oleobject/label/
---
## OleObject.Label property

Obtient et définit l'étiquette d'affichage de l'objet ole lié.

```csharp
public string Label { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyLabelDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un objet OLE avec un libellé
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleIndex];
            oleObject.Label = "label_nameです";

            // Enregistrer et recharger le Workbook
            string outputPath = "output.xlsx";
            workbook.Save(outputPath);
            
            // Vérifier la propriété du libellé
            Workbook loadedWorkbook = new Workbook(outputPath);
            OleObject loadedOleObject = loadedWorkbook.Worksheets[0].OleObjects[0];
            Console.WriteLine("OLE Object Label: " + loadedOleObject.Label);
        }
    }
}
```

### Voir aussi

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


