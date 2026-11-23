---
title: "LoadOptions.LoadOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur LoadOptions. Crée des options de chargement du fichier"
type: docs
url: /fr/net/aspose.cells/loadoptions/loadoptions/
---
## LoadOptions() {#constructor}

Crée une option de chargement du fichier.

```csharp
public LoadOptions()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsMethodSharpctorDemo
    {
        public static void Run()
        {
            string tempCsvPath = "temp_input.csv";

            try
            {
                // Créez un contenu CSV d'exemple
                File.WriteAllText(tempCsvPath, "Name,Age\nJohn,30\nJane,25");

                // Démontrer le constructeur par défaut
                LoadOptions defaultOptions = new LoadOptions();
                Console.WriteLine("Default LoadFormat: " + defaultOptions.LoadFormat);

                // Démontrer le constructeur avec le paramètre LoadFormat
                LoadOptions csvOptions = new LoadOptions(LoadFormat.Csv);
                Console.WriteLine("CSV LoadFormat: " + csvOptions.LoadFormat);

                // Charger le fichier CSV avec les options spécifiées
                Workbook workbook = new Workbook(tempCsvPath, csvOptions);

                // Vérifier que les données ont été chargées correctement
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine($"Cell A1: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"Cell B2: {worksheet.Cells["B2"].StringValue}");

                // Enregistrer au format XLSX pour démontrer la conversion
                workbook.Save("CsvToExcel.xlsx");
                Console.WriteLine("CSV file successfully loaded and converted to XLSX");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
            finally
            {
                if (File.Exists(tempCsvPath))
                    File.Delete(tempCsvPath);
            }
        }
    }
}
```

### Voir aussi

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## LoadOptions(LoadFormat) {#constructor_1}

Crée une option de chargement du fichier.

```csharp
public LoadOptions(LoadFormat loadFormat)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| loadFormat | LoadFormat | Le format de chargement. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            string tempCsvPath = "temp_input.csv";
            
            try
            {
                // Créez un contenu CSV d'exemple
                File.WriteAllText(tempCsvPath, "Column1,Column2\nData1,Data2");

                // Créer LoadOptions avec LoadFormat.Csv
                LoadOptions options = new LoadOptions(LoadFormat.Csv);

                // Charger le fichier CSV avec les options créées
                Workbook workbook = new Workbook(tempCsvPath, options);

                // Démontrer le chargement réussi en lisant la cellule
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine($"A1 cell value: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"B2 cell value: {worksheet.Cells["B2"].StringValue}");

                // Enregistrer au format XLSX pour montrer la capacité de conversion
                workbook.Save("CsvLoadedAsExcel.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during CSV loading: {ex.Message}");
            }
            finally
            {
                if (File.Exists(tempCsvPath))
                    File.Delete(tempCsvPath);
            }
        }
    }
}
```

### Voir aussi

* enum [LoadFormat](../../loadformat/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


