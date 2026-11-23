---
title: "Class HeaderFooterCommand"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.HeaderFooterCommand. Représente la commande d'en-tête/pied de page"
type: docs
url: /fr/net/aspose.cells/headerfootercommand/
---
## HeaderFooterCommand class

Représente la commande d'en-tête/pied de page

```csharp
public class HeaderFooterCommand
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Font](../../aspose.cells/headerfootercommand/font/) { get; } | Obtient la police de la valeur de la commande. |
| [Text](../../aspose.cells/headerfootercommand/text/) { get; } | Obtient le texte de la commande. |
| [Type](../../aspose.cells/headerfootercommand/type/) { get; } | Obtient le type de commande d'en-tête/pied de page. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassHeaderFooterCommandDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accédez à PageSetup et définissez l'en-tête avec des commandes
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.SetHeader(1, "&D&\"Arial\"sdfsdfsdfsdf");
            
            // Obtenir les commandes d'en-tête
            HeaderFooterCommand[] commands = pageSetup.GetCommands(pageSetup.GetHeader(1));
            
            // Afficher les types de commande et le texte
            Console.WriteLine("Command 1 Type: " + commands[0].Type);
            Console.WriteLine("Command 2 Type: " + commands[1].Type);
            Console.WriteLine("Command 2 Text: " + commands[1].Text);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


