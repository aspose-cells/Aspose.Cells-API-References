---
title: "ConversionUtility.Convert"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ConversionUtility. Convertit les fichiers Excel en d'autres formats"
type: docs
url: /fr/net/aspose.cells.utility/conversionutility/convert/
---
## Convert(string, string) {#convert_1}

Convertit les fichiers Excel vers d'autres formats.

```csharp
public static void Convert(string source, string saveAs)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| source | String | Le nom du fichier source. |
| saveAs | String | Le nom du fichier attendu. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class ConversionUtilityMethodConvertWithStringStringDemo
    {
        public static void Run()
        {
            // Initialiser les chemins des fichiers source et de destination
            string sourcePath = "source.xlsx";
            string destPath = "output.pdf";
            // Convertir le fichier Excel en PDF
            ConversionUtility.Convert(sourcePath, destPath);

            Console.WriteLine("Conversion completed successfully.");
        }
    }
}
```

### Voir aussi

* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)

---

## Convert(string, LoadOptions, string, SaveOptions) {#convert}

Convertit les fichiers Excel vers d'autres formats.

```csharp
public static void Convert(string source, LoadOptions loadOptions, string saveAs, 
    SaveOptions saveOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| source | String | Le nom du fichier source. |
| loadOptions | LoadOptions | Les options de chargement du fichier source. |
| saveAs | String | Le nom du fichier attendu. |
| saveOptions | SaveOptions | Les options d'enregistrement du fichier. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ConversionUtilityMethodConvertWithStringLoadOptionsStringSaveOptDemo
    {
        public static void Run()
        {
            // Chemins des fichiers source et de destination
            string sourceFile = "input.csv";
            string outputFile = "output.xlsx";

            // Créer un fichier CSV d'exemple pour la démonstration
            System.IO.File.WriteAllText(sourceFile, "Name,Age\nJohn,30\nAlice,25");

            try
            {
                // Créer des options de chargement pour le fichier CSV
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                
                // Créer des options d'enregistrement pour le fichier XLSX
                SaveOptions saveOptions = new OoxmlSaveOptions();

                // Convertir CSV en XLSX avec les options spécifiées
                ConversionUtility.Convert(sourceFile, loadOptions, outputFile, saveOptions);

                Console.WriteLine($"File converted successfully from {sourceFile} to {outputFile}");
                
                // Vérifier la conversion en chargeant le fichier de sortie
                Workbook workbook = new Workbook(outputFile);
                Console.WriteLine($"Output file contains {workbook.Worksheets.Count} worksheet(s)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
            finally
            {
                // Nettoyez les fichiers temporaires
                if (System.IO.File.Exists(sourceFile))
                {
                    System.IO.File.Delete(sourceFile);
                }
            }
        }
    }
}
```

### Voir aussi

* class [LoadOptions](../../../aspose.cells/loadoptions/)
* class [SaveOptions](../../../aspose.cells/saveoptions/)
* class [ConversionUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


