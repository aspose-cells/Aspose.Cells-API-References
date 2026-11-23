---
title: "XmlSaveOptions.SheetIndexes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété XmlSaveOptions. Représente les index des feuilles exportées"
type: docs
url: /fr/net/aspose.cells/xmlsaveoptions/sheetindexes/
---
## XmlSaveOptions.SheetIndexes property

Représente les index des feuilles exportées.

```csharp
public int[] SheetIndexes { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec plusieurs feuilles
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Remplir des données dans toutes les feuilles
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue("Data in " + sheet.Name);
            }

            // Créer une instance de XmlSaveOptions
            XmlSaveOptions options = new XmlSaveOptions();

            // Exporter initialement toutes les feuilles (SheetIndexes est nul)
            Console.WriteLine("Initial SheetIndexes value: " + (options.SheetIndexes == null ? "null (all sheets)" : string.Join(",", options.SheetIndexes)));

            // Définir pour n'exporter que la première et la troisième feuille (index 0 et 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // Enregistrer avec uniquement les feuilles sélectionnées
            workbook.Save("XmlExportSelectedSheets.xml", options);

            // Modifier pour n'exporter que la deuxième feuille (index 1)
            options.SheetIndexes = new int[] { 1 };

            // Enregistrer avec une sélection de feuilles différente
            workbook.Save("XmlExportSingleSheet.xml", options);

            // Définir SheetIndexes à null pour exporter toutes les feuilles
            options.SheetIndexes = null;
            workbook.Save("XmlExportAllSheets.xml", options);
        }
    }
}
```

### Voir aussi

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


