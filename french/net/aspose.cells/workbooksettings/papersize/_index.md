---
title: "WorkbookSettings.PaperSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient et définit la taille de papier d'impression par défaut"
type: docs
url: /fr/net/aspose.cells/workbooksettings/papersize/
---
## WorkbookSettings.PaperSize property

Obtient et définit la taille de papier d'impression par défaut.

```csharp
public PaperSizeType PaperSize { get; set; }
```

### Remarques

S'il n'y a aucun paramètre concernant la taille du papier, MS Excel utilisera les paramètres de l'imprimante par défaut.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyPaperSizeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Définir la taille du papier à A5
            workbook.Settings.PaperSize = PaperSizeType.PaperA5;
            
            // Vérifier que la taille du papier est correctement définie dans la première feuille de calcul
            Console.WriteLine("Paper size: " + workbook.Worksheets[0].PageSetup.PaperSize);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* enum [PaperSizeType](../../papersizetype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


