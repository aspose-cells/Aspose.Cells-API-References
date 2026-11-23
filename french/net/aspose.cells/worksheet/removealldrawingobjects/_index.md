---
title: "Worksheet.RemoveAllDrawingObjects"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Supprime tous les objets graphiques de cette feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/removealldrawingobjects/
---
## Worksheet.RemoveAllDrawingObjects method

Supprime tous les objets de dessin de cette feuille de calcul.

```csharp
public void RemoveAllDrawingObjects()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRemoveAllDrawingObjectsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter quelques objets graphiques à la feuille de calcul
            worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 50);
            worksheet.Shapes.AddLine(1, 0, 5, 100, 5, 150);
            
            // Enregistrer avant de supprimer les objets
            workbook.Save("BeforeRemove.xlsx", SaveFormat.Xlsx);
            
            // Supprimer tous les objets graphiques
            worksheet.RemoveAllDrawingObjects();
            
            // Enregistrer après avoir supprimé les objets
            workbook.Save("AfterRemove.xlsx", SaveFormat.Xlsx);
            
            // Libérer le classeur
            workbook.Dispose();
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


