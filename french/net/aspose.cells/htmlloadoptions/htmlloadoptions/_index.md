---
title: "HtmlLoadOptions.HtmlLoadOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur HtmlLoadOptions. Crée des options de chargement du fichier"
type: docs
url: /fr/net/aspose.cells/htmlloadoptions/htmlloadoptions/
---
## HtmlLoadOptions() {#constructor}

Crée une option de chargement du fichier.

```csharp
public HtmlLoadOptions()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Créez des options de chargement HTML en utilisant le constructeur
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;

            // Chargez le fichier HTML avec les options
            Workbook workbook = new Workbook("example.html", loadOptions);

            // Accédez aux données du HTML chargé
            Worksheet worksheet = workbook.Worksheets[0];
            Console.WriteLine("B1 Cell Value: " + worksheet.Cells["B1"].StringValue);
            Console.WriteLine("B3 Cell Value: " + worksheet.Cells["B3"].StringValue);
            Console.WriteLine("B4 Cell Value: " + worksheet.Cells["B4"].StringValue);
        }
    }
}
```

### Voir aussi

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HtmlLoadOptions(LoadFormat) {#constructor_1}

Crée une option de chargement du fichier.

```csharp
public HtmlLoadOptions(LoadFormat loadFormat)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| loadFormat | LoadFormat | Le format de chargement. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // Créez une instance de HtmlLoadOptions en utilisant le constructeur avec le paramètre LoadFormat
                HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);

                // Définissez certaines propriétés de HtmlLoadOptions
                loadOptions.AutoFitColsAndRows = true;
                loadOptions.SupportDivTag = true;
                loadOptions.DeleteRedundantSpaces = true;

                // Créez un classeur en utilisant les options de chargement
                Workbook workbook = new Workbook("input.html", loadOptions);

                // Accéder à la première feuille de calcul
                Worksheet worksheet = workbook.Worksheets[0];

                // Afficher certaines informations sur le HTML chargé
                Console.WriteLine("HTML loaded successfully with LoadFormat.Html");
                Console.WriteLine($"Worksheet name: {worksheet.Name}");
                Console.WriteLine($"Cells count: {worksheet.Cells.MaxDataRow + 1} rows x {worksheet.Cells.MaxDataColumn + 1} columns");

                // Enregistrez le classeur
                workbook.Save("HtmlLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading HTML file: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [LoadFormat](../../loadformat/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


