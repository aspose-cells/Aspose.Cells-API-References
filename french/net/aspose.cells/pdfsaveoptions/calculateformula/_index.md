---
title: "PdfSaveOptions.CalculateFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PdfSaveOptions. Indique s'il faut calculer les formules avant d'enregistrer le fichier pdf"
type: docs
url: /fr/net/aspose.cells/pdfsaveoptions/calculateformula/
---
## PdfSaveOptions.CalculateFormula property

Indique s'il faut calculer les formules avant d'enregistrer le fichier pdf.

```csharp
public bool CalculateFormula { get; set; }
```

### Remarques

La valeur par défaut est false.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Créer un classeur avec des données d'exemple et des formules
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir des valeurs et des formules
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Créer des options d'enregistrement PDF avec le calcul des formules
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.CalculateFormula = true;

            // Enregistrer dans le flux mémoire
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, pdfSaveOptions);
                
                // Réinitialiser la position du flux et vérifier le contenu
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string content = reader.ReadToEnd();
                    Console.WriteLine("PDF contains formula results: " + content.Contains("30"));
                }
            }
        }
    }
}
```

### Voir aussi

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


