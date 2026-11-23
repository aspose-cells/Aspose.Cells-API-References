---
title: "XlsbSaveOptions.XlsbSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur XlsbSaveOptions. Crée des options d'enregistrement de fichier xlsb"
type: docs
url: /fr/net/aspose.cells/xlsbsaveoptions/xlsbsaveoptions/
---
## XlsbSaveOptions() {#constructor}

Crée les options d'enregistrement de fichier xlsb.

```csharp
public XlsbSaveOptions()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsbSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("Test Value");

            XlsbSaveOptions saveOptions = new XlsbSaveOptions();
            saveOptions.ExportAllColumnIndexes = true;

            workbook.Save("output.xlsb", saveOptions);
        }
    }
}
```

### Voir aussi

* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XlsbSaveOptions(SaveFormat) {#constructor_1}

Crée les options d'enregistrement de fichier xlsb.

```csharp
[Obsolete("Use XlsbSaveOptions() constructor instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public XlsbSaveOptions(SaveFormat saveFormat)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | Le format d'enregistrement. Il doit être xlsb. |

### Remarques

NOTE : Ce constructeur est maintenant obsolète. Au lieu de cela, veuillez utiliser le constructeur XlsbSaveOptions(). Cette propriété sera supprimée 12 mois plus tard depuis janvier 2021. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XlsbSaveOptionsMethodSharpctorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Using XlsbSaveOptions";

            try
            {
                // Créez XlsbSaveOptions en utilisant le constructeur avec le paramètre SaveFormat
                XlsbSaveOptions saveOptions = new XlsbSaveOptions(SaveFormat.Xlsb);

                // Définissez des propriétés supplémentaires si nécessaire
                saveOptions.ExportAllColumnIndexes = true;

                // Enregistrez le classeur avec les options d'enregistrement spécifiées
                workbook.Save("XlsbSaveOptionsDemo.xlsb", saveOptions);

                Console.WriteLine("Workbook saved successfully with XlsbSaveOptions");
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

* enum [SaveFormat](../../saveformat/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


