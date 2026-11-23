---
title: "PageSetup.GetCommands"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PageSetup. Récupère toutes les commandes d'en-tête ou de pied de page"
type: docs
url: /fr/net/aspose.cells/pagesetup/getcommands/
---
## PageSetup.GetCommands method

Obtient toutes les commandes d'en-tête ou de pied de page.

```csharp
public HeaderFooterCommand[] GetCommands(string headerFooterScript)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| headerFooterScript | String | Le script d'en-tête/pied de page |

### Valeur de retour

Renvoie toutes les commandes d'en-tête ou de pied de page.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetCommandsWithStringDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir l'en-tête avec des commandes
            string header = "&D&\"Arial\"&12sdfsdfsdfsdf";
            worksheet.PageSetup.SetHeader(1, header);
            
            // Obtenir les commandes d'en-tête
            HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(header);
            
            // Afficher les types de commande et le texte
            foreach (HeaderFooterCommand cmd in commands)
            {
                Console.WriteLine($"Type: {cmd.Type}, Text: {cmd.Text}");
            }
        }
    }
}
```

### Voir aussi

* class [HeaderFooterCommand](../../headerfootercommand/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


