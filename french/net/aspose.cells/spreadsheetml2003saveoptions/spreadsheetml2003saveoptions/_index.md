---
title: "SpreadsheetML2003SaveOptions.SpreadsheetML2003SaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur SpreadsheetML2003SaveOptions. Crée les options pour enregistrer un fichier Excel 2003 spreadml"
type: docs
url: /fr/net/aspose.cells/spreadsheetml2003saveoptions/spreadsheetml2003saveoptions/
---
## SpreadsheetML2003SaveOptions() {#constructor}

Crée les options pour enregistrer un fichier spreadml Excel 2003.

```csharp
public SpreadsheetML2003SaveOptions()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez à la première feuille de calcul et ajoutez des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            // Créer SpreadsheetML2003SaveOptions avec le constructeur
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            
            // Définir les options
            saveOptions.LimitAsXls = true;
            saveOptions.ExportColumnIndexOfCell = true;

            // Enregistrer avec les options
            workbook.Save("output.xml", saveOptions);
            
            Console.WriteLine("File saved with SpreadsheetML2003SaveOptions");
        }
    }
}
```

### Voir aussi

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SpreadsheetML2003SaveOptions(SaveFormat) {#constructor_1}

Crée les options pour enregistrer un fichier spreadml Excel 2003.

```csharp
[Obsolete("Use SpreadsheetML2003SaveOptions() constructor instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SpreadsheetML2003SaveOptions(SaveFormat saveFormat)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | Le format d'enregistrement. |

### Remarques

NOTE : Ce constructeur est maintenant obsolète. À la place, veuillez utiliser le constructeur SpreadsheetML2003SaveOptions(). Cette propriété sera supprimée 12 mois plus tard depuis janvier 2021. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SpreadsheetML2003SaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue(123.45);

            try
            {
                // Appeler la méthode #ctor avec le paramètre SaveFormat
                SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();

                // Définir certaines propriétés des options d'enregistrement
                saveOptions.IsIndentedFormatting = true;
                saveOptions.LimitAsXls = false;
                saveOptions.ExportColumnIndexOfCell = true;

                Console.WriteLine("SpreadsheetML2003SaveOptions created successfully with SaveFormat parameter");

                // Enregistrer le classeur en utilisant les options d'enregistrement créées
                workbook.Save("SpreadsheetML2003Output.xml", saveOptions);
                Console.WriteLine("Workbook saved successfully with SpreadsheetML2003SaveOptions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SpreadsheetML2003SaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [SaveFormat](../../saveformat/)
* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


