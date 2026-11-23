---
title: "WorksheetCollection.OleSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorksheetCollection. Obtient et définit la taille affichée lorsque le fichier Workbook est utilisé comme objet Ole"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/olesize/
---
## WorksheetCollection.OleSize property

Obtient et définit la taille affichée lorsque le fichier Workbook est utilisé comme objet Ole.

```csharp
public object OleSize { get; set; }
```

### Remarques

Null signifie aucune configuration de taille ole.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyOleSizeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Définir la taille OLE pour la collection de feuilles de calcul
            workbook.Worksheets.SetOleSize(0, 10, 0, 10);
            
            // Accéder et afficher les propriétés de taille OLE
            CellArea oleSize = (CellArea)workbook.Worksheets.OleSize;
            Console.WriteLine("OLE Size Range:");
            Console.WriteLine($"StartRow: {oleSize.StartRow}, EndRow: {oleSize.EndRow}");
            Console.WriteLine($"StartColumn: {oleSize.StartColumn}, EndColumn: {oleSize.EndColumn}");
            
            // Enregistrez le classeur
            workbook.Save("OleSizeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


