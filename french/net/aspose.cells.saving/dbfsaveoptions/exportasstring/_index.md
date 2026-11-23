---
title: "DbfSaveOptions.ExportAsString"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DbfSaveOptions. Indique si l'exportation se fait en tant que valeur de chaîne"
type: docs
url: /fr/net/aspose.cells.saving/dbfsaveoptions/exportasstring/
---
## DbfSaveOptions.ExportAsString property

Indique si l'exportation se fait sous forme de valeur chaîne

```csharp
public bool ExportAsString { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class DbfSaveOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple avec des types mixtes
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("TextValue");

            // Créer une instance DbfSaveOptions
            DbfSaveOptions options = new DbfSaveOptions();

            // Afficher la valeur actuelle de ExportAsString
            Console.WriteLine("Current ExportAsString value: " + options.ExportAsString);

            // Définir ExportAsString sur true (toutes les valeurs seront exportées en tant que chaînes)
            options.ExportAsString = true;
            Console.WriteLine("ExportAsString set to: " + options.ExportAsString);

            // Enregistrer avec ExportAsString = true
            workbook.Save("ExportAsStringTrue.dbf", options);

            // Définir ExportAsString sur false (les valeurs conserveront leurs types d'origine)
            options.ExportAsString = false;
            Console.WriteLine("ExportAsString set to: " + options.ExportAsString);

            // Enregistrer avec ExportAsString = false
            workbook.Save("ExportAsStringFalse.dbf", options);
        }
    }
}
```

### Voir aussi

* class [DbfSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


