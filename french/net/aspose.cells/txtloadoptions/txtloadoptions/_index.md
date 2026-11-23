---
title: "TxtLoadOptions.TxtLoadOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur TxtLoadOptions. Crée les options pour charger un fichier texte"
type: docs
url: /fr/net/aspose.cells/txtloadoptions/txtloadoptions/
---
## TxtLoadOptions() {#constructor}

Crée les options de chargement d'un fichier texte.

```csharp
public TxtLoadOptions()
```

### Remarques

Le type de fichier chargé par défaut est CSV.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Créez un nouveau TxtLoadOptions en utilisant le constructeur
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            
            // Définissez le séparateur pour le fichier CSV
            loadOptions.Separator = ',';
            
            // Créez un classeur avec les options de chargement
            Workbook workbook = new Workbook("example.csv", loadOptions);
            
            // Affichez certaines informations du fichier chargé
            Console.WriteLine("Worksheet count: " + workbook.Worksheets.Count);
            Console.WriteLine("First cell value: " + workbook.Worksheets[0].Cells["A1"].Value);
        }
    }
}
```

### Voir aussi

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## TxtLoadOptions(LoadFormat) {#constructor_1}

Crée les options de chargement d'un fichier texte.

```csharp
public TxtLoadOptions(LoadFormat loadFormat)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| loadFormat | LoadFormat | Le format de chargement |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class TxtLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            // Créez un contenu CSV d'exemple et un fichier temporaire
            string csvData = "Column1,Column2,Column3\nData1,Data2,Data3";
            string tempFile = Path.GetTempFileName();
            File.WriteAllText(tempFile, csvData);

            try
            {
                // Créez un TxtLoadOptions avec LoadFormat.Csv
                TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
                loadOptions.Separator = ',';
                loadOptions.HasTextQualifier = true;

                // Chargez le CSV en utilisant les options configurées
                Workbook workbook = new Workbook(tempFile, loadOptions);
                Worksheet worksheet = workbook.Worksheets[0];

                // Démontrez les données chargées
                Console.WriteLine($"A1 Cell Value: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"B2 Cell Value: {worksheet.Cells["B2"].StringValue}");

                // Enregistrer le classeur traité
                workbook.Save("TxtLoadOptionsCtorDemoOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing constructor: {ex.Message}");
            }
            finally
            {
                // Nettoyer le fichier temporaire
                if (File.Exists(tempFile))
                {
                    File.Delete(tempFile);
                }
            }
        }
    }
}
```

### Voir aussi

* enum [LoadFormat](../../loadformat/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


