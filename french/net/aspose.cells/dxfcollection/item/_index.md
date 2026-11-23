---
title: "DxfCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DxfCollection. Obtient l'élément à l'index spécifié"
type: docs
url: /fr/net/aspose.cells/dxfcollection/item/
---
## DxfCollection indexer

Obtient l'élément à l'index spécifié.

```csharp
public Style this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'index spécifié. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DxfCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à DxfCollection depuis le classeur
            DxfCollection dxfCollection = workbook.Worksheets.Dxfs;

            // Créer un nouveau style (impossible d'ajouter directement à DxfCollection car il n'a pas de méthode Add)
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            // Le style est automatiquement ajouté à la collection lors de sa création

            // Obtenir le premier élément de DxfCollection en utilisant la propriété Item
            Style firstStyle = dxfCollection[0];
            Console.WriteLine("First style font name: " + firstStyle.Font.Name);

            // Modifiez le style via la propriété Item (car elle renvoie une référence)
            firstStyle.Font.Color = System.Drawing.Color.Red;
            firstStyle.Font.IsBold = true;

            // Vérifier le changement
            Console.WriteLine("Modified style font color: " + dxfCollection[0].Font.Color);
            Console.WriteLine("Modified style font bold: " + dxfCollection[0].Font.IsBold);

            // Appliquez le style à une cellule pour voir l'effet
            worksheet.Cells["A1"].PutValue("DxfCollection Property Item Demo");
            worksheet.Cells["A1"].SetStyle(dxfCollection[0]);

            // Enregistrer le résultat
            workbook.Save("DxfCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [DxfCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


