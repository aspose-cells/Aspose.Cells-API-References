---
title: "Workbook.RemovePersonalInformation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Supprime les informations personnelles"
type: docs
url: /fr/net/aspose.cells/workbook/removepersonalinformation/
---
## Workbook.RemovePersonalInformation method

Supprime les informations personnelles.

```csharp
public void RemovePersonalInformation()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemovePersonalInformationDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Ajouter un commentaire avec les informations de l'auteur
            int commentIndex = sheet.Comments.Add("A1");
            sheet.Comments[commentIndex].Note = "Sample comment";
            sheet.Comments[commentIndex].Author = "Test Author";
            
            // Afficher les informations d'origine de l'auteur
            Console.WriteLine("Before removal - Comment Author: " + sheet.Comments[commentIndex].Author);
            
            // Supprimer les informations personnelles
            wb.RemovePersonalInformation();
            
            // Enregistrez le classeur
            wb.Save("output.xlsx", SaveFormat.Xlsx);
            
            // Recharger pour vérifier la suppression
            Workbook wb2 = new Workbook("output.xlsx");
            Console.WriteLine("After removal - Comment Author: " + wb2.Worksheets[0].Comments[commentIndex].Author);
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


