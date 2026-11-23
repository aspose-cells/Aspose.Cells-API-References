---
title: "WorksheetCollection.SetOleSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "WorksheetCollection méthode. Définit la taille affichée lorsque le fichier Workbook est utilisé comme objet Ole"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/setolesize/
---
## WorksheetCollection.SetOleSize method

Définit la taille affichée lorsque le fichier classeur est utilisé comme objet Ole.

```csharp
public void SetOleSize(int startRow, int endRow, int startColumn, int endColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Indice de ligne de départ. |
| endRow | Int32 | Indice de ligne de fin. |
| startColumn | Int32 | Indice de colonne de départ. |
| endColumn | Int32 | Indice de colonne de fin. |

### Remarques

Cette méthode est généralement utilisée pour ajuster la taille d'affichage dans un fichier ppt ou doc.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodSetOleSizeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Définir la taille OLE pour les feuilles de calcul
            workbook.Worksheets.SetOleSize(0, 10, 0, 10);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            // Vérifier la taille OLE
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            CellArea oleSize = (CellArea)loadedWorkbook.Worksheets.OleSize;
            Console.WriteLine("OLE Size - StartRow: {0}, EndRow: {1}, StartColumn: {2}, EndColumn: {3}", 
                oleSize.StartRow, oleSize.EndRow, oleSize.StartColumn, oleSize.EndColumn);
        }
    }
}
```

### Voir aussi

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


