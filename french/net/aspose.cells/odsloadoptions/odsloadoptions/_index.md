---
title: "OdsLoadOptions.OdsLoadOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur OdsLoadOptions. Représente les options de chargement du fichier ods"
type: docs
url: /fr/net/aspose.cells/odsloadoptions/odsloadoptions/
---
## OdsLoadOptions() {#constructor}

Représente les options de chargement du fichier ODS.

```csharp
public OdsLoadOptions()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Créer OdsLoadOptions en utilisant le constructeur
            OdsLoadOptions loadOptions = new OdsLoadOptions();
            
            // Définir le style de lien hypertexte pour utiliser les paramètres par défaut d'Excel
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;
            
            // Charger le fichier ODS avec les options de chargement
            Workbook workbook = new Workbook("example.ods", loadOptions);
            
            // Enregistrer au format XLSX
            workbook.Save("output.xlsx");
            
            // Vérifier que le style de lien hypertexte a été appliqué
            Console.WriteLine("Hyperlink style color: " + 
                workbook.Worksheets[0].Cells["B1"].GetStyle().Font.Color);
        }
    }
}
```

### Voir aussi

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OdsLoadOptions(LoadFormat) {#constructor_1}

Représente les options de chargement du fichier ODS.

```csharp
public OdsLoadOptions(LoadFormat type)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | LoadFormat | Le type de format de chargement. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class OdsLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            // Créer un fichier ODS d'exemple s'il n'existe pas
            string inputFile = "input.ods";
            if (!File.Exists(inputFile))
            {
                using (Workbook sampleWorkbook = new Workbook())
                {
                    sampleWorkbook.Worksheets[0].Hyperlinks.Add("A1", 1, 1, "https://example.com");
                    sampleWorkbook.Save(inputFile, SaveFormat.Ods);
                }
            }

            // Créer OdsLoadOptions avec le paramètre LoadFormat
            OdsLoadOptions loadOptions = new OdsLoadOptions(LoadFormat.Ods);
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;

            try
            {
                // Charger le classeur avec les options de chargement créées
                using (Workbook workbook = new Workbook(inputFile, loadOptions))
                {
                    Console.WriteLine($"Hyperlink style applied: {loadOptions.ApplyExcelDefaultStyleToHyperlink}");
                    
                    // Enregistrer pour démontrer le chargement réussi
                    workbook.Save("OdsLoadOptionsCtorDemo.xlsx");
                }
            }
            catch (FileNotFoundException)
            {
                Console.WriteLine("Error: Created sample file missing - please verify permissions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading ODS file: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [LoadFormat](../../loadformat/)
* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


