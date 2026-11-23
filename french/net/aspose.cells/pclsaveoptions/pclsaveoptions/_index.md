---
title: "PclSaveOptions.PclSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur de PclSaveOptions. Crée les options pour enregistrer un fichier pcl"
type: docs
url: /fr/net/aspose.cells/pclsaveoptions/pclsaveoptions/
---
## PclSaveOptions constructor

Crée les options pour enregistrer le fichier pcl.

```csharp
public PclSaveOptions()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("PCL Save Options Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates PclSaveOptions constructor");
            
            try
            {
                // Appelez la méthode #ctor pour créer une instance de PclSaveOptions
                PclSaveOptions pclOptions = new PclSaveOptions();
                
                // Configurez des options supplémentaires si nécessaire
                pclOptions.AddPrinterFont("Arial", "ArialPCL");
                
                Console.WriteLine("PclSaveOptions created successfully");
                
                // Enregistrez le classeur avec les options PCL
                workbook.Save("PclSaveOptionsDemo.pcl", pclOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating PclSaveOptions: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


