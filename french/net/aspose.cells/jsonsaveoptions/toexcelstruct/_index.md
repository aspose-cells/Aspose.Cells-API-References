---
title: "JsonSaveOptions.ToExcelStruct"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété JsonSaveOptions. Indique s’il faut convertir en structure JSON du fichier Excel"
type: docs
url: /fr/net/aspose.cells/jsonsaveoptions/toexcelstruct/
---
## JsonSaveOptions.ToExcelStruct property

Indique s’il faut convertir en structure JSON du fichier Excel.

```csharp
public bool ToExcelStruct { get; set; }
```

### Remarques

Uniquement pour convertir la plage en JSON.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyToExcelStructDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Créer une plage à exporter
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

            // Configurer les options d'enregistrement JSON avec ToExcelStruct
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ToExcelStruct = true;

            // Exportez la plage vers JSON
            string json = range.ToJson(saveOptions);
            Console.WriteLine(json);
        }
    }
}
```

### Voir aussi

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


