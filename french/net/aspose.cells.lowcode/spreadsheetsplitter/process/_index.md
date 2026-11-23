---
title: "SpreadsheetSplitter.Process"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SpreadsheetSplitter. Divise le fichier modèle donné en plusieurs parties"
type: docs
url: /fr/net/aspose.cells.lowcode/spreadsheetsplitter/process/
---
## Process(string, string) {#process_1}

Divise le fichier modèle fourni en plusieurs parties.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| templateFile | String | Le fichier modèle à diviser |
| resultFile | String | Le fichier résultant (modèle de nom) |

### Remarques

Les fichiers de sortie seront construits à partir du fichier résultant spécifié en ajoutant le numéro de séquence de la feuille et de la partie découpée. Par exemple, si le fichier de sortie spécifié est Split.xlsx, les fichiers générés seront Split_0_0.xlsx, Split_0_1.xlsx, ..., Split_1_0.xlsx, ...

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetSplitterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec plusieurs feuilles de calcul
            Workbook templateWorkbook = new Workbook();
            Worksheet sheet1 = templateWorkbook.Worksheets.Add("SalesData");
            sheet1.Cells["A1"].PutValue("Product");
            Worksheet sheet2 = templateWorkbook.Worksheets.Add("Inventory");
            sheet2.Cells["A1"].PutValue("test data");

            // Enregistrer comme fichier modèle
            string templatePath = "SplitterTemplate.xlsx";
            templateWorkbook.Save(templatePath, SaveFormat.Xlsx);

            // Définir le modèle de sortie du résultat
            string resultPattern = "SplitResult_";
            
            try
            {
                // Traiter le modèle directement en utilisant la méthode statique
                SpreadsheetSplitter.Process(templatePath, resultPattern);
                
                Console.WriteLine($"Spreadsheet split successfully using pattern: {resultPattern}");
                Console.WriteLine("Check output directory for split files");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during spreadsheet splitting: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SpreadsheetSplitter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeSplitOptions) {#process}

Divise le fichier de feuille de calcul en plusieurs parties.

```csharp
public static void Process(LowCodeSplitOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | LowCodeSplitOptions | Options pour diviser la feuille de calcul |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class SpreadsheetSplitterMethodProcessWithLowCodeSplitOptionsDemo
    {
        public static void Run()
        {

            // Initialiser les options de division
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions
            {
                LoadOptions = new LowCodeLoadOptions { InputFile = "split.xlsx" },
                SaveOptionsProvider = new CustomLowCodeSaveOptionsProvider()
            };

            try
            {
                // Exécuter la division de la feuille de calcul en utilisant une méthode statique
                SpreadsheetSplitter.Process(splitOptions);
                
                Console.WriteLine($"Spreadsheet split successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Split operation failed: {ex.Message}");
            }
        }
    }

    // Implémentation concrète de AbstractLowCodeSaveOptionsProvider
    public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override void Finish(LowCodeSaveOptions part)
        {
            base.Finish(part);
        }
        // Implémentez la méthode abstraite requise
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            LowCodeSaveOptions result = new LowCodeSaveOptions();
            result.SaveFormat = SaveFormat.Xlsx;
            result.OutputFile = partInfo.SheetName + "_split.xlsx";
            Console.WriteLine(result.OutputFile);
            return result;
        }
    }
}
```

### Voir aussi

* class [LowCodeSplitOptions](../../lowcodesplitoptions/)
* class [SpreadsheetSplitter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


