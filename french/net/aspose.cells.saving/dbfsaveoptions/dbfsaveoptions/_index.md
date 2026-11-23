---
title: "DbfSaveOptions.DbfSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur DbfSaveOptions. Les options d'enregistrement du fichier .dbf"
type: docs
url: /fr/net/aspose.cells.saving/dbfsaveoptions/dbfsaveoptions/
---
## DbfSaveOptions constructor

Les options d'enregistrement du fichier .dbf.

```csharp
public DbfSaveOptions()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class DbfSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            try
            {
                // Créer une instance DbfSaveOptions en utilisant le constructeur
                DbfSaveOptions saveOptions = new DbfSaveOptions();
                
                // Définir les propriétés des options d'enregistrement
                saveOptions.ExportAsString = true;
                
                // Enregistrer le classeur avec les options d'enregistrement DBF
                workbook.Save("DbfSaveOptionsDemo.dbf", saveOptions);
                
                Console.WriteLine("DBF file saved successfully with ExportAsString option set to true");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving DBF file: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [DbfSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


