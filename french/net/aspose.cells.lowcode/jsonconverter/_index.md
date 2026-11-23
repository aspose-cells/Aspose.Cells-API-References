---
title: "Classe JsonConverter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.LowCode.JsonConverter. Convertisseur pour la conversion entre la structure de données json et d'autres formats de feuilles de calcul."
type: docs
url: /fr/net/aspose.cells.lowcode/jsonconverter/
---
## JsonConverter class

Convertisseur pour la conversion entre la structure de données json et d'autres formats de fichiers de feuille de calcul.

```csharp
public class JsonConverter
```

## Méthodes

| Nom | Description |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/jsonconverter/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions) | Convertit entre les données json et d'autres formats de feuilles de calcul. |
| static [Process](../../aspose.cells.lowcode/jsonconverter/process/#process_1)(string, string) | Convertit le fichier modèle donné entre json et d'autres formats. |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassJsonConverterDemo
    {
        public static void Run()
        {
            string jsonFilePath = "data.json";
            string excelFilePath = "res.xlsx";

            try
            {
                // Convertir JSON en Excel en utilisant Aspose.Cells.LowCode.JsonConverter
                JsonConverter.Process(jsonFilePath, excelFilePath);

                Console.WriteLine("Conversion completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


