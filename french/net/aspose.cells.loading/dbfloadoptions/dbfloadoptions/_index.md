---
title: "DbfLoadOptions.DbfLoadOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur DbfLoadOptions. Les options"
type: docs
url: /fr/net/aspose.cells.loading/dbfloadoptions/dbfloadoptions/
---
## DbfLoadOptions constructor

Les options.

```csharp
public DbfLoadOptions()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;
    using System;

    public class DbfLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            try
            {
                // Créer une instance DbfLoadOptions en utilisant la méthode #ctor
                DbfLoadOptions loadOptions = new DbfLoadOptions();

                // Créer un classeur avec les options de chargement DBF
                Workbook workbook = new Workbook("sample.dbf", loadOptions);

                // Accéder à la première feuille de calcul
                Worksheet worksheet = workbook.Worksheets[0];

                // Afficher certaines données du fichier DBF chargé
                Console.WriteLine("Data loaded from DBF file:");
                Console.WriteLine(worksheet.Cells["A1"].StringValue);

                // Enregistrer le classeur au format Excel
                workbook.Save("DbfLoadOptionsCtorDemo.xlsx", SaveFormat.Xlsx);
                Console.WriteLine("File saved successfully with DBF data");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DbfLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [DbfLoadOptions](../)
* namespace [Aspose.Cells.Loading](../../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../../)


