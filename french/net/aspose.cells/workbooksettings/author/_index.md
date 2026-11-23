---
title: "WorkbookSettings.Author"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient et définit l'auteur du fichier"
type: docs
url: /fr/net/aspose.cells/workbooksettings/author/
---
## WorkbookSettings.Author property

Obtient et définit l'auteur du fichier.

```csharp
public string Author { get; set; }
```

### Remarques

Ce n'est pas défini, vérifiez d'abord [`Author`](../../../aspose.cells.properties/builtindocumentpropertycollection/author/) puis vérifiez l'utilisateur de Environment.

### Exemples

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAuthorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez aux WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Définir la propriété author
            settings.Author = "John Doe";

            // Ajouter des données d'exemple pour démontrer la fonctionnalité du classeur
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Sample Workbook");
            sheet.Cells["A2"].PutValue("Created by: " + settings.Author);
            sheet.Cells["A3"].PutValue(DateTime.Now.ToString());

            // Enregistrez le classeur
            workbook.Save("AuthorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


