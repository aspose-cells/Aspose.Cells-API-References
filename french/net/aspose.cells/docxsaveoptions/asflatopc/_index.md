---
title: "DocxSaveOptions.AsFlatOpc"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DocxSaveOptions. Indique si l’enregistrement se fait sous forme de fichier OPC plat qui peut être généré par Open XML SDK"
type: docs
url: /fr/net/aspose.cells/docxsaveoptions/asflatopc/
---
## DocxSaveOptions.AsFlatOpc property

Indique s'il faut enregistrer en tant que fichier opc plat qui peut être généré par Open XML SDK

```csharp
public bool AsFlatOpc { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul et ajouter des données d’exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Flat OPC Demo";

            try
            {
                // Initialiser DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Afficher la valeur par défaut de la propriété AsFlatOpc
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // Définir AsFlatOpc sur true pour démontrer son utilisation
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // Enregistrer le classeur au format DOCX avec les options configurées
                workbook.Save("AsFlatOpcDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with AsFlatOpc option.");
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

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


