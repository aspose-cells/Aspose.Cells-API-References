---
title: "LoadOptions.ParsingPivotCachedRecords"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "LoadOptions property. Indique si l’analyse des enregistrements de cache de tableau croisé dynamique est effectuée lors du chargement du fichier. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/loadoptions/parsingpivotcachedrecords/
---
## LoadOptions.ParsingPivotCachedRecords property

Indique s'il faut analyser les enregistrements mis en cache du tableau croisé dynamique lors du chargement du fichier. La valeur par défaut est false.

```csharp
public bool ParsingPivotCachedRecords { get; set; }
```

### Remarques

S’applique uniquement aux fichiers Excel Xlsx, Xltx, Xltm, Xlsm et xlsb

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyParsingPivotCachedRecordsDemo
    {
        public static void Run()
        {
            // Créer des options de chargement CSV
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
            
            // Activer l’analyse des enregistrements de cache de tableau croisé dynamique
            loadOptions.ParsingPivotCachedRecords = true;
            
            // Chargez le classeur avec les options
            Workbook workbook = new Workbook("example.csv", loadOptions);
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "PivotData";
            
            // Créer un tableau croisé dynamique (démontrant que la propriété est définie)
            int pivotIndex = worksheet.PivotTables.Add("A1:C10", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Enregistrez le classeur
            workbook.Save("PivotTableOutput.xlsx");
        }
    }
}
```

### Voir aussi

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


