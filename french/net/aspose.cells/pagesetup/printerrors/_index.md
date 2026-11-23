---
title: "PageSetup.PrintErrors"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Spécifie le type d'erreur d'impression affichée"
type: docs
url: /fr/net/aspose.cells/pagesetup/printerrors/
---
## PageSetup.PrintErrors property

Spécifie le type d'erreur d'impression affichée.

```csharp
public PrintErrorsType PrintErrors { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintErrorsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet sheet = workbook.Worksheets[0];
            
            // Définir les erreurs d'impression pour qu'elles s'affichent comme vides
            sheet.PageSetup.PrintErrors = PrintErrorsType.PrintErrorsBlank;
            Console.WriteLine("PrintErrors set to: " + sheet.PageSetup.PrintErrors);
            
            // Modifier les erreurs d'impression pour qu'elles s'affichent sous forme de tirets
            sheet.PageSetup.PrintErrors = PrintErrorsType.PrintErrorsDash;
            Console.WriteLine("PrintErrors changed to: " + sheet.PageSetup.PrintErrors);
            
            // Enregistrez le classeur
            workbook.Save("PrintErrorsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PrintErrorsType](../../printerrorstype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


