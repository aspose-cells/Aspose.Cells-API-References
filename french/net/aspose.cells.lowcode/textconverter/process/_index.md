---
title: "TextConverter.Process"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode TextConverter. Convertit le fichier modèle donné entre des fichiers texte et d'autres formats"
type: docs
url: /fr/net/aspose.cells.lowcode/textconverter/process/
---
## Process(string, string) {#process_1}

Convertit le fichier modèle donné entre des fichiers basés sur du texte et d'autres formats.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| templateFile | String | Le fichier modèle à convertir |
| resultFile | String | Le fichier résultant |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class TextConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            string inputFile = "input.csv";
            string outputFile = "output.xlsx";

            // Créer un fichier CSV d'exemple
            File.WriteAllText(inputFile, $"Column1,Column2{Environment.NewLine}Data1,Data2{Environment.NewLine}Data3,Data4");

            try
            {
                // Appelez la méthode statique Process directement sans instancier TextConverter
                TextConverter.Process(inputFile, outputFile);
                
                Console.WriteLine($"Process method successfully converted {inputFile} to {outputFile}");
                Console.WriteLine($"Converted file exists: {File.Exists(outputFile)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process method: {ex.Message}");
            }
            finally
            {
                // Nettoyer les fichiers temporaires
                if (File.Exists(inputFile))
                {
                    File.Delete(inputFile);
                }
            }
        }
    }
}
```

### Voir aussi

* class [TextConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Convertit le format de fichier entre les formats basés sur du texte et d'autres formats de feuilles de calcul

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Options d'entrée et de chargement |
| saveOptions | LowCodeSaveOptions | Options de sortie et d'enregistrement |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class TextConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // Créer un fichier texte d'exemple
            string inputText = "Sample text content";
            string inputPath = "input.txt";
            File.WriteAllText(inputPath, inputText);

            // Traitez le fichier texte avec les options LowCode
            using (FileStream inputStream = new FileStream(inputPath, FileMode.Open))
            {
                TextConverter.Process(
                    new LowCodeLoadOptions() { InputStream = inputStream },
                    new LowCodeSaveOptions()
                    {
                        OutputFile = "output.txt"
                    }
                );
            }

            Console.WriteLine("Text processing completed successfully.");
        }
    }
}
```

### Voir aussi

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [TextConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


