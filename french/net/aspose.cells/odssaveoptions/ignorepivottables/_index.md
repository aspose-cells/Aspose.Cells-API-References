---
title: "OdsSaveOptions.IgnorePivotTables"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OdsSaveOptions. Indique si les tableaux croisés dynamiques sont enregistrés"
type: docs
url: /fr/net/aspose.cells/odssaveoptions/ignorepivottables/
---
## OdsSaveOptions.IgnorePivotTables property

Indique s’il faut enregistrer les tableaux croisés dynamiques.

```csharp
public bool IgnorePivotTables { get; set; }
```

### Remarques

La fonctionnalité de tableau croisé dynamique d’OpenOffice possède moins de paramètres comparée à Excel, ainsi leurs résultats de tableau croisé dynamique présentent de nombreuses différences. Parfois il vaut mieux ignorer ces tableaux croisés dynamiques lors de l’enregistrement d’un fichier .ods.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class OdsSaveOptionsPropertyIgnorePivotTablesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(3000);

            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = workbook.Worksheets[0].PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Créer une instance OdsSaveOptions
            OdsSaveOptions saveOptions = new OdsSaveOptions();

            // Afficher la valeur actuelle de IgnorePivotTables
            Console.WriteLine("Current IgnorePivotTables value: " + saveOptions.IgnorePivotTables);

            // Définir pour ignorer les tableaux croisés dynamiques lors de l’enregistrement
            saveOptions.IgnorePivotTables = true;

            // Enregistrer avec les tableaux croisés dynamiques ignorés
            workbook.Save("IgnorePivotTablesDemo_Ignored.ods", saveOptions);

            // Définir pour inclure les tableaux croisés dynamiques lors de l’enregistrement
            saveOptions.IgnorePivotTables = false;

            // Enregistrer avec les tableaux croisés dynamiques inclus
            workbook.Save("IgnorePivotTablesDemo_Included.ods", saveOptions);
        }
    }
}
```

### Voir aussi

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


