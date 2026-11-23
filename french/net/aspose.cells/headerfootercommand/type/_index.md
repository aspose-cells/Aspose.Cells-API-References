---
title: "HeaderFooterCommand.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HeaderFooterCommand. Obtient le type de la commande d'en-tête/pied de page"
type: docs
url: /fr/net/aspose.cells/headerfootercommand/type/
---
## HeaderFooterCommand.Type property

Obtient le type de commande d'en-tête/pied de page.

```csharp
public HeaderFooterCommandType Type { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HeaderFooterCommandPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir l’en-tête avec différents types de commande
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.SetHeader(0, "&D&\"Arial\"&12sdfsdfsdfsdf");
            
            // Obtenir les commandes d'en-tête
            HeaderFooterCommand[] commands = pageSetup.GetCommands(pageSetup.GetHeader(0));
            
            // Démontrer l'utilisation de la propriété Type
            Console.WriteLine("Command 0 Type: " + commands[0].Type); // CurrentDate
            Console.WriteLine("Command 1 Type: " + commands[1].Type); // Text
            Console.WriteLine("Command 1 Text: " + commands[1].Text); // sdfsdfsdfsdf
        }
    }
}
```

### Voir aussi

* enum [HeaderFooterCommandType](../../headerfootercommandtype/)
* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


