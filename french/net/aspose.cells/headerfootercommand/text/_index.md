---
title: "HeaderFooterCommand.Text"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HeaderFooterCommand. Obtient le texte de la commande"
type: docs
url: /fr/net/aspose.cells/headerfootercommand/text/
---
## HeaderFooterCommand.Text property

Obtient le texte de la commande.

```csharp
public string Text { get; }
```

### Remarques

Valide uniquement pour HeaderFooterCommandType.Text.

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class HeaderFooterCommandPropertyTextDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir l'en-tête avec la commande texte
            worksheet.PageSetup.SetHeader(1, "&\"Arial\"&12&KFF0000Sample Text Header");
            
            // Obtenir les commandes d'en-tête
            HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(worksheet.PageSetup.GetHeader(1));
            
            // Afficher les informations sur la commande texte
            foreach (HeaderFooterCommand cmd in commands)
            {
                if (cmd.Type == HeaderFooterCommandType.Text)
                {
                    Console.WriteLine("Text command found:");
                    Console.WriteLine("Text: " + cmd.Text);
                    Console.WriteLine("Font: " + cmd.Font);
                    Console.WriteLine("Color: " + ColorTranslator.ToHtml(cmd.Font.Color));
                }
            }
            
            // Enregistrez le classeur
            workbook.Save("HeaderFooterTextDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


