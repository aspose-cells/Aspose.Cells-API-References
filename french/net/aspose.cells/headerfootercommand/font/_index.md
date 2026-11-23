---
title: "HeaderFooterCommand.Font"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HeaderFooterCommand. Obtient la police de la valeur de la commande"
type: docs
url: /fr/net/aspose.cells/headerfootercommand/font/
---
## HeaderFooterCommand.Font property

Obtient la police de la valeur de la commande.

```csharp
public Font Font { get; }
```

### Remarques

Inutile pour HeaderFooterCommandType.Picture.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HeaderFooterCommandPropertyFontDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la configuration de page pour l'en-tête/pied de page
            PageSetup pageSetup = worksheet.PageSetup;

            // Définir un en-tête avec du texte qui aura une HeaderFooterCommand
            pageSetup.SetHeader(0, "&\"Arial\"&12&BThis is a header");

            // Obtenir le script d'en-tête
            string headerScript = pageSetup.GetHeader(0);

            // Obtenir les commandes d'en-tête
            HeaderFooterCommand[] commands = pageSetup.GetCommands(headerScript);

            // Trouver la commande texte (en supposant que c'est la première)
            if (commands.Length > 0 && commands[0].Type == HeaderFooterCommandType.Text)
            {
                HeaderFooterCommand textCommand = commands[0];
                
                // Accéder à la propriété Font (lecture seule)
                Font font = textCommand.Font;
                
                // Afficher les propriétés actuelles de la police
                Console.WriteLine("Current Font:");
                Console.WriteLine($"Name: {font.Name}");
                Console.WriteLine($"Size: {font.Size}");
                Console.WriteLine($"Bold: {font.IsBold}");
                Console.WriteLine($"Color: {font.Color}");

                // Comme la police est en lecture seule, nous ne pouvons pas assigner un nouvel objet Font,
                // mais nous pouvons modifier les propriétés de la police existante
                font.Name = "Times New Roman";
                font.Size = 14;
                font.IsBold = false;
                font.Color = System.Drawing.Color.Blue;

                // Enregistrez le classeur pour voir les modifications
                workbook.Save("HeaderFooterFontDemo.xlsx");

                Console.WriteLine("\nModified Font:");
                Console.WriteLine($"Name: {font.Name}");
                Console.WriteLine($"Size: {font.Size}");
                Console.WriteLine($"Bold: {font.IsBold}");
                Console.WriteLine($"Color: {font.Color}");
            }
        }
    }
}
```

### Voir aussi

* class [Font](../../font/)
* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


