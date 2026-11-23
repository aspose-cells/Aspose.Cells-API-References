---
title: "LowCodeSplitOptions.SaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeSplitOptions. Options d'enregistrement pour enregistrer les parties découpées"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesplitoptions/saveoptions/
---
## LowCodeSplitOptions.SaveOptions property

Options d'enregistrement pour enregistrer les parties découpées.

```csharp
public LowCodeSaveOptions SaveOptions { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertySaveOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et ajouter des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Créer une instance de LowCodeSplitOptions
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();

            // Afficher la valeur initiale de SaveOptions (null par défaut)
            Console.WriteLine("Initial SaveOptions value: " + (splitOptions.SaveOptions == null ? "null" : splitOptions.SaveOptions.ToString()));

            // Créer et configurer LowCodeSaveOptions pour le format PDF
            LowCodeSaveOptions pdfSaveOptions = new LowCodeSaveOptions();
            pdfSaveOptions.SaveFormat = SaveFormat.Pdf;

            // Attribuer les options d'enregistrement aux SplitOptions
            splitOptions.SaveOptions = pdfSaveOptions;

            // Afficher la valeur mise à jour de SaveOptions
            Console.WriteLine("Updated SaveOptions SaveFormat: " + splitOptions.SaveOptions.SaveFormat);

            // Exemple de scénario d'utilisation : le fractionnement du classeur enregistrerait les parties au format PDF
            // (Le code réel de division dépendrait de l'implémentation de l'API Aspose.Cells.LowCode)
            // LowCodeEngine.Split(workbook, splitOptions, "output_directory/");
            
            // Enregistrez le classeur original à des fins de démonstration (non affecté par SplitOptions)
            workbook.Save("LowCodeSplitOptionsPropertySaveOptionsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


