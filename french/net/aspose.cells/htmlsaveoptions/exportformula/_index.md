---
title: "HtmlSaveOptions.ExportFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique s'il faut exporter la formule lors de l'enregistrement du fichier en html. La valeur par défaut est true. Si vous souhaitez importer le html généré dans Excel, veuillez conserver la valeur par défaut"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/exportformula/
---
## HtmlSaveOptions.ExportFormula property

Indique si l'exportation des formules est activée lors de l'enregistrement du fichier en html. La valeur par défaut est true. Si vous souhaitez importer le html généré dans excel, veuillez conserver la valeur par défaut.

```csharp
public bool ExportFormula { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportFormulaDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple et une formule
            worksheet.Cells["A1"].PutValue("Value 1");
            worksheet.Cells["B1"].PutValue("Value 2");
            worksheet.Cells["C1"].Formula = "=A1+B1";
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["C2"].Formula = "=A2+B2";

            // Enregistrez avec ExportFormula = true
            HtmlSaveOptions options1 = new HtmlSaveOptions();
            options1.ExportFormula = true;
            workbook.Save("output_with_formulas.html", options1);

            // Enregistrez avec ExportFormula = false
            HtmlSaveOptions options2 = new HtmlSaveOptions();
            options2.ExportFormula = false;
            workbook.Save("output_without_formulas.html", options2);

            // Vérifier les résultats
            string htmlWithFormulas = File.ReadAllText("output_with_formulas.html");
            string htmlWithoutFormulas = File.ReadAllText("output_without_formulas.html");

            Console.WriteLine("HTML with formulas contains formula: " + 
                htmlWithFormulas.Contains("=A2+B2"));
            Console.WriteLine("HTML without formulas contains formula: " + 
                htmlWithoutFormulas.Contains("=A2+B2"));
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


