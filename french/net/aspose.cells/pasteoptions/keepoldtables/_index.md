---
title: "PasteOptions.KeepOldTables"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PasteOptions. Conserve les tables dans la plage de destination"
type: docs
url: /fr/net/aspose.cells/pasteoptions/keepoldtables/
---
## PasteOptions.KeepOldTables property

Conserve les tableaux dans la plage de destination.

```csharp
public bool KeepOldTables { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PasteOptionsPropertyKeepOldTablesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Créer une feuille de calcul d'exemple avec des données
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Source Data";
            worksheet.Cells["B1"].Value = "Table Data";

            try
            {
                // Créer une instance de PasteOptions
                PasteOptions pasteOptions = new PasteOptions();

                // Afficher la valeur par défaut de la propriété KeepOldTables
                Console.WriteLine("Default KeepOldTables value: " + pasteOptions.KeepOldTables);

                // Définir KeepOldTables sur true
                pasteOptions.KeepOldTables = true;
                Console.WriteLine("KeepOldTables set to: " + pasteOptions.KeepOldTables);

                // Créer des plages pour l'opération de copie
                Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:B1");
                Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("A3:B3");

                // Copier avec l'option KeepOldTables
                targetRange.Copy(sourceRange, pasteOptions);

                // Enregistrez le classeur
                workbook.Save("KeepOldTablesDemo.xlsx");
                Console.WriteLine("Workbook saved with KeepOldTables option applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


