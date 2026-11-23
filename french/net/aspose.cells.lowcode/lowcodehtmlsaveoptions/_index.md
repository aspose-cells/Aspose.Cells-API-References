---
title: "Classe LowCodeHtmlSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.LowCode.LowCodeHtmlSaveOptions. Options pour enregistrer le HTML de manière low‑code"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/
---
## LowCodeHtmlSaveOptions class

Options pour enregistrer le html de manière low‑code.

```csharp
public class LowCodeHtmlSaveOptions : LowCodeSaveOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [LowCodeHtmlSaveOptions](lowcodehtmlsaveoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [HtmlOptions](../../aspose.cells.lowcode/lowcodehtmlsaveoptions/htmloptions/) { get; set; } | Les options générales pour l’enregistrement du HTML. |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Obtient et définit le fichier (avec le chemin si nécessaire) pour enregistrer les données générées. Lors de la définition de cette propriété avec une valeur différente de null ou d'une chaîne vide, [`OutputStream`](../lowcodesaveoptions/outputstream/) sera ignoré.(Hérité de [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Obtient et définit le flux pour écrire les données générées. Lors de la définition de cette propriété avec une valeur différente de null, [`OutputFile`](../lowcodesaveoptions/outputfile/) sera ignoré.(Hérité de [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodehtmlsaveoptions/saveformat/) { get; set; } | Obtient et définit le format de la feuille de calcul. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeHtmlSaveOptionsDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Widget");
            worksheet.Cells["B2"].PutValue(29.99);

            // Créer et configurer LowCodeHtmlSaveOptions
            LowCodeHtmlSaveOptions saveOptions = new LowCodeHtmlSaveOptions
            {
                HtmlOptions = new HtmlSaveOptions()
                {
                    ExportWorksheetCSSSeparately = false,
                    ExportImagesAsBase64 = true
                }
            };

            // Enregistrer le classeur avec les options HTML configurées en utilisant le paramètre d’options d’enregistrement
            workbook.Save("LowCodeHtmlExport.html", saveOptions.HtmlOptions);

            Console.WriteLine("HTML file saved successfully with low code options.");
        }
    }
}
```

### Voir aussi

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


