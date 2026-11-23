---
title: "LowCodeSaveOptions.SaveFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeSaveOptions. Obtient et définit le format d'enregistrement pour la sortie. Généralement, pour un processus spécifique en mode low‑code, seuls certains formats spécifiques sont autorisés. Veuillez spécifier le format correct pour le processus correspondant, sinon un résultat inattendu ou même une exception peut survenir."
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesaveoptions/saveformat/
---
## LowCodeSaveOptions.SaveFormat property

Obtient et définit le format d'enregistrement pour la sortie. En général, pour un processus spécifique en low‑code, seuls certains formats spécifiques sont autorisés. Veuillez spécifier le format correct pour le processus correspondant, sinon un résultat inattendu ou même une exception peut survenir.

```csharp
public virtual SaveFormat SaveFormat { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);

            // Initialiser LowCodeSaveOptions avec différents formats
            LowCodeSaveOptions excelOptions = new LowCodeSaveOptions();
            LowCodeSaveOptions pdfOptions = new LowCodeSaveOptions();

            // Configurer les options d'enregistrement Excel
            excelOptions.SaveFormat = SaveFormat.Xlsx;
            excelOptions.OutputFile = "output_excel.xlsx";

            // Configurer les options d'enregistrement PDF
            pdfOptions.SaveFormat = SaveFormat.Pdf;
            pdfOptions.OutputFile = "output_pdf.pdf";

            // Démontrer l'enregistrement au format original
            Console.WriteLine($"Saving as {excelOptions.SaveFormat}");
            workbook.Save(excelOptions.OutputFile, excelOptions.SaveFormat);

            // Démontrer le changement de format et le réenregistrement
            Console.WriteLine($"Changing format to {pdfOptions.SaveFormat}");
            Console.WriteLine($"Saving as {pdfOptions.SaveFormat}");
            workbook.Save(pdfOptions.OutputFile, pdfOptions.SaveFormat);

            Console.WriteLine("Files saved successfully with different formats.");
        }
    }
}
```

### Voir aussi

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


