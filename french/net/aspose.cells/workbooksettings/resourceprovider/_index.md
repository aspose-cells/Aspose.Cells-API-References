---
title: "WorkbookSettings.ResourceProvider"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient et définit le fournisseur de flux pour les ressources externes telles que le chargement de données d'image pour une image de type LinkToFile"
type: docs
url: /fr/net/aspose.cells/workbooksettings/resourceprovider/
---
## WorkbookSettings.ResourceProvider property

Obtient et définit le fournisseur de flux pour les ressources externes, comme le chargement de données d'image pour une image de type "LinkToFile".

```csharp
public IStreamProvider ResourceProvider { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyResourceProviderDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une forme d'exemple pour démontrer le fournisseur de ressources
            worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 200);
            
            // Définir le fournisseur de ressources
            workbook.Settings.ResourceProvider = new MemoryStreamProvider();
            
            // Enregistrer la forme en tant qu'image en utilisant le fournisseur de ressources
            string outputPath = "output_shape.png";
            worksheet.Shapes[0].ToImage(outputPath, new ImageOrPrintOptions());
            
            Console.WriteLine("Shape saved as image using ResourceProvider.");
        }
    }

    public class MemoryStreamProvider : IStreamProvider
    {
        public void CloseStream(StreamProviderOptions options)
        {
            options.Stream.Close();
        }

        public void InitStream(StreamProviderOptions options)
        {
            options.Stream = new FileStream(options.DefaultPath, FileMode.Create);
        }
    }
}
```

### Voir aussi

* interface [IStreamProvider](../../istreamprovider/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


