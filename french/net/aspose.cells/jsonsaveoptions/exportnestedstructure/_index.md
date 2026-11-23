---
title: "JsonSaveOptions.ExportNestedStructure"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété JsonSaveOptions. Exporté comme une structure Json hiérarchique parent‑enfant"
type: docs
url: /fr/net/aspose.cells/jsonsaveoptions/exportnestedstructure/
---
## JsonSaveOptions.ExportNestedStructure property

Exporté sous forme de structure JSON hiérarchique parent-enfant.

```csharp
public bool ExportNestedStructure { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportNestedStructureDemo
    {
        public static void Run()
        {
            // Créer un classeur d’exemple avec des données imbriquées
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer une structure de données imbriquée
            worksheet.Cells["A1"].PutValue("Parent");
            worksheet.Cells["B1"].PutValue("Child");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Fruits");
            worksheet.Cells["B3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Vegetables");
            worksheet.Cells["B4"].PutValue("Carrot");

            // Configurer les options d’enregistrement JSON avec ExportNestedStructure
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportNestedStructure = true;
            saveOptions.AlwaysExportAsJsonObject = true;

            // Enregistrer avec une structure imbriquée
            string outputPath = "output_nested.json";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("Workbook exported to JSON with nested structure. Output: " + outputPath);
        }
    }
}
```

### Voir aussi

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


