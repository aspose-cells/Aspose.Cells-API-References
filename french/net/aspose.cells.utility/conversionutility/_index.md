---
title: "Classe ConversionUtility"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Utility.ConversionUtility. Représente un utilitaire permettant de convertir des fichiers vers d'autres formats"
type: docs
url: /fr/net/aspose.cells.utility/conversionutility/
---
## ConversionUtility class

Représente l'utilitaire permettant de convertir des fichiers vers d'autres formats.

```csharp
public class ConversionUtility
```

## Méthodes

| Nom | Description |
| --- | --- |
| static [Convert](../../aspose.cells.utility/conversionutility/convert/#convert_1)(string, string) | Convertit les fichiers Excel vers d'autres formats. |
| static [Convert](../../aspose.cells.utility/conversionutility/convert/#convert)(string, LoadOptions, string, SaveOptions) | Convertit les fichiers Excel vers d'autres formats. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;
    using System.IO;

    public class UtilityClassConversionUtilityDemo
    {
        public static void Run()
        {
            // Créez un fichier CSV d'exemple pour la conversion
            string sourceFile = "sample.csv";
            string outputFile = "converted.xlsx";

            try
            {
                // Créez un contenu CSV d'exemple
                File.WriteAllText(sourceFile, "Product,Price,Quantity\nApple,1.50,100\nBanana,0.75,150\nOrange,1.25,120");

                // Convertissez CSV en XLSX en utilisant la méthode de conversion statique
                ConversionUtility.Convert(sourceFile, outputFile);

                Console.WriteLine($"Successfully converted {sourceFile} to {outputFile}");

                // Vérifiez la conversion en vérifiant si le fichier de sortie existe
                if (File.Exists(outputFile))
                {
                    Console.WriteLine("Output file created successfully");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
            finally
            {
                // Nettoyez les fichiers temporaires
                if (File.Exists(sourceFile))
                {
                    File.Delete(sourceFile);
                }
                if (File.Exists(outputFile))
                {
                    File.Delete(outputFile);
                }
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


