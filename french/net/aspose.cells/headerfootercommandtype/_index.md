---
title: "Énumération HeaderFooterCommandType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.HeaderFooterCommandType. Représente le type de commande d’en-tête et de pied de page"
type: docs
url: /fr/net/aspose.cells/headerfootercommandtype/
---
## HeaderFooterCommandType enumeration

Représente le type de commande d'en-tête et de pied de page.

```csharp
public enum HeaderFooterCommandType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Text | `0` | Le texte. |
| CurrentPage | `1` | Numéro de page actuel |
| Pagecount | `2` | Nombre de pages |
| CurrentDate | `3` | Date actuelle |
| CurrentTime | `4` | Heure actuelle |
| SheetName | `5` | Nom de la feuille |
| FileName | `6` | Nom de fichier sans le chemin |
| FilePath | `7` | Chemin du fichier sans le nom de fichier |
| Picture | `8` | Image |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassHeaderFooterCommandTypeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Définir l’en-tête avec différents types de commande
                worksheet.PageSetup.SetHeader(0, "&[Page] of &[Pages] - &[Date] - &[Time] - &[File]");

                // Récupérer les commandes d’en-tête
                string headerScript = worksheet.PageSetup.GetHeader(0);
                HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(headerScript);

                // Démontrer les différentes valeurs de HeaderFooterCommandType
                foreach (HeaderFooterCommand cmd in commands)
                {
                    Console.WriteLine($"Command Type: {cmd.Type}");

                    // Vérifier des types de commande spécifiques
                    if (cmd.Type == HeaderFooterCommandType.CurrentPage)
                    {
                        Console.WriteLine("Found CurrentPage command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.Pagecount)
                    {
                        Console.WriteLine("Found Pagecount command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.CurrentDate)
                    {
                        Console.WriteLine("Found CurrentDate command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.CurrentTime)
                    {
                        Console.WriteLine("Found CurrentTime command");
                    }
                    else if (cmd.Type == HeaderFooterCommandType.FileName)
                    {
                        Console.WriteLine("Found FileName command");
                    }
                }

                // Enregistrer le classeur pour démontrer la configuration de l’en-tête
                workbook.Save("HeaderFooterCommandTypeDemo.xlsx");
                Console.WriteLine("HeaderFooterCommandType demonstration completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with HeaderFooterCommandType: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


