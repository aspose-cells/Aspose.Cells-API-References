---
title: "OleObjectCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OleObjectCollection. Obtient l'élément OleObject à l'index spécifié"
type: docs
url: /fr/net/aspose.cells.drawing/oleobjectcollection/item/
---
## OleObjectCollection indexer

Obtient l'élément [`OleObject`](../../oleobject/) à l'index spécifié.

```csharp
public OleObject this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice à base zéro de l'élément. |

### Valeur de retour

L’élément à l’index spécifié.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter des données d'image d'exemple
            byte[] binaryImg = File.ReadAllBytes("image1.png");
            
            // Ajouter un objet OLE à la première feuille de calcul
            int idxOle = workbook.Worksheets[0].OleObjects.Add(0, 0, 60, 60, binaryImg);
            
            // Accéder à l'objet OLE en utilisant la propriété Item
            OleObject objOle = workbook.Worksheets[0].OleObjects[idxOle];
            
            // Définir les propriétés de l'objet intégré
            byte[] binaryXlsx = File.ReadAllBytes("example.xlsx");
            objOle.SetEmbeddedObject(false, binaryXlsx, "SampleFile.xlsx", true, "Excel.Sheet", false);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            // Vérifier le fichier enregistré
            Workbook savedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("OLE Object Source: " + savedWorkbook.Worksheets[0].OleObjects[0].ObjectSourceFullName);
        }
    }
}
```

### Voir aussi

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


