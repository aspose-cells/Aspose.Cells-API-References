---
title: "PptxSaveOptions.PptxSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur de PptxSaveOptions. Représente les options d’enregistrement pptx"
type: docs
url: /fr/net/aspose.cells/pptxsaveoptions/pptxsaveoptions/
---
## PptxSaveOptions() {#constructor}

Représente les options d'enregistrement pptx.

```csharp
public PptxSaveOptions()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Visible Data");
            worksheet.Cells["A2"].PutValue("Hidden Data");
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            
            // Masquer la deuxième ligne
            worksheet.Cells.Rows[1].IsHidden = true;

            // Créer un PptxSaveOptions en utilisant le constructeur
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.IgnoreHiddenRows = true;

            // Enregistrer le classeur au format PPTX avec des options
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("Workbook saved to PPTX with hidden rows ignored.");
        }
    }
}
```

### Voir aussi

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## PptxSaveOptions(bool) {#constructor_1}

Représente les options d'enregistrement d'un fichier .pptx.

```csharp
public PptxSaveOptions(bool saveAsImage)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| saveAsImage | Boolean | Si True, le classeur sera converti en quelques images du fichier .pptx. Si False, le classeur sera converti en quelques tableaux du fichier .pptx. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Slides;
    using System;

    public class PptxSaveOptionsMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            try
            {
                // Appeler la méthode #ctor avec un paramètre booléen
                bool saveAsImage = true;
                PptxSaveOptions options = new PptxSaveOptions(saveAsImage);

                // Définir des propriétés supplémentaires
                options.IgnoreHiddenRows = true;
                options.ExportViewType = SlideViewType.View;

                // Enregistrer le classeur avec les options PPTX
                workbook.Save("PptxSaveOptionsCtorDemo.pptx", options);

                Console.WriteLine("PptxSaveOptions constructor executed successfully with parameter: " + saveAsImage);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PptxSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


