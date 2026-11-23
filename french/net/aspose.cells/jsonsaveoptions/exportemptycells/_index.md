---
title: "JsonSaveOptions.ExportEmptyCells"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété JsonSaveOptions. Indique s'il faut exporter les cellules vides comme null"
type: docs
url: /fr/net/aspose.cells/jsonsaveoptions/exportemptycells/
---
## JsonSaveOptions.ExportEmptyCells property

Indique s’il faut exporter les cellules vides en tant que null.

```csharp
public bool ExportEmptyCells { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportEmptyCellsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir les données avec quelques cellules vides
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue(2.99); // B2 is intentionally left empty

            // Créer JsonSaveOptions avec ExportEmptyCells défini sur false
            JsonSaveOptions options = new JsonSaveOptions
            {
                ExportEmptyCells = false
            };

            // Enregistrer au JSON - les cellules vides seront ignorées
            workbook.Save("output_skip_empty.json", options);

            // Modifier ExportEmptyCells à true
            options.ExportEmptyCells = true;

            // Enregistrer à nouveau - les cellules vides seront incluses
            workbook.Save("output_include_empty.json", options);
        }
    }
}
```

### Voir aussi

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


