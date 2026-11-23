---
title: "EbookLoadOptions.EbookLoadOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur EbookLoadOptions. Crée une option pour charger le fichier ebook"
type: docs
url: /fr/net/aspose.cells/ebookloadoptions/ebookloadoptions/
---
## EbookLoadOptions() {#constructor}

Crée une option pour charger le fichier ebook.

```csharp
public EbookLoadOptions()
```

### Exemples

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class EbookLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Créez une instance de EbookLoadOptions en utilisant le constructeur
            EbookLoadOptions options = new EbookLoadOptions();

            // Définir quelques propriétés de base
            options.Password = "secure123";
            options.Encoding = Encoding.UTF8;
            options.LoadFormulas = true;
            
            // Chargez un fichier ebook avec les options spécifiées
            Workbook workbook = new Workbook("sample.epub", options);
            
            // Enregistrer en tant que fichier Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [EbookLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## EbookLoadOptions(LoadFormat) {#constructor_1}

Crée une option de chargement du fichier ebook.

```csharp
public EbookLoadOptions(LoadFormat loadFormat)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| loadFormat | LoadFormat | Le format de chargement |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class EbookLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // Créez une instance de EbookLoadOptions avec le paramètre LoadFormat
                EbookLoadOptions options = new EbookLoadOptions(LoadFormat.Epub);

                // Afficher la confirmation
                Console.WriteLine("EbookLoadOptions created successfully with LoadFormat.Epub");

                // Exemple d'utilisation : chargez un classeur avec ces options
                Workbook workbook = new Workbook("sample.epub", options);
                Console.WriteLine("Workbook loaded successfully with EbookLoadOptions");

                // Enregistrer le résultat
                workbook.Save("EbookLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EbookLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [LoadFormat](../../loadformat/)
* class [EbookLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


