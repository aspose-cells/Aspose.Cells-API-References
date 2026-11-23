---
title: "PclSaveOptions.EmbedFont"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PclSaveOptions. Indique s'il faut intégrer la police dans le fichier Pcl de sortie"
type: docs
url: /fr/net/aspose.cells/pclsaveoptions/embedfont/
---
## PclSaveOptions.EmbedFont property

Indique s'il faut incorporer la police dans le fichier Pcl de sortie.

```csharp
public bool EmbedFont { get; set; }
```

### Remarques

La valeur par défaut est true.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsPropertyEmbedFontDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et ajouter des données d’exemple
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demonstrating EmbedFont property");
            sheet.Cells["A2"].PutValue(DateTime.Now);

            try
            {
                // Créez des options d'enregistrement PCL
                PclSaveOptions pclOptions = new PclSaveOptions();

                // Lisez et affichez la valeur actuelle de la propriété EmbedFont
                Console.WriteLine("Current EmbedFont value: " + pclOptions.EmbedFont);

                // (Optionnel) Si la propriété est modifiable, vous pourriez la définir, mais nous ne faisons que la lire ici
                // pclOptions.EmbedFont = true;

                // Enregistrez le classeur au format PCL en utilisant les options
                workbook.Save("EmbedFontDemo.pcl", pclOptions);

                Console.WriteLine("Workbook saved successfully with EmbedFont demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Voir aussi

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


