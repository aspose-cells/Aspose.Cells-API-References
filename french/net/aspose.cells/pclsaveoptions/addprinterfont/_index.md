---
title: "PclSaveOptions.AddPrinterFont"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PclSaveOptions. Ajoute des informations sur la police déjà ajoutée à l'imprimante par le fabricant"
type: docs
url: /fr/net/aspose.cells/pclsaveoptions/addprinterfont/
---
## PclSaveOptions.AddPrinterFont method

Ajoute des informations sur la police déjà ajoutée à l'imprimante par le fabricant.

```csharp
public void AddPrinterFont(string fontFullName, string fontPclName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fontFullName | String | Nom complet de la police (par ex. "Times New Roman Bold Italic") utilisé dans le fichier source. |
| fontPclName | String | Nom de la police qui sera utilisée dans le document Pcl de sortie. |

### Remarques

Il existe 52 polices qui doivent être intégrées dans toute imprimante selon la spécification Pcl. Cependant, les fabricants peuvent ajouter d'autres polices à leurs appareils.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsMethodAddPrinterFontWithStringStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez du texte à la feuille de calcul pour démontrer l'utilisation des polices
            worksheet.Cells["A1"].PutValue("This text will use the added printer font");
            
            // Créez des options d'enregistrement PCL
            PclSaveOptions pclSaveOptions = new PclSaveOptions();
            
            try
            {
                // Appelez la méthode AddPrinterFont avec des noms de police spécifiques
                pclSaveOptions.AddPrinterFont("Arial", "ArialPCL");
                pclSaveOptions.AddPrinterFont("Times New Roman", "TimesPCL");
                
                Console.WriteLine("AddPrinterFont method executed successfully with parameters (String, String)");
                
                // Enregistrez le classeur avec les options PCL
                workbook.Save("PclWithAddedPrinterFonts.pcl", pclSaveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddPrinterFont method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


