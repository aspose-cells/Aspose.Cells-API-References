---
title: "PageSetup.PrinterSettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Obtient et définit les paramètres de l'imprimante par défaut"
type: docs
url: /fr/net/aspose.cells/pagesetup/printersettings/
---
## PageSetup.PrinterSettings property

Obtient et définit les paramètres de l'imprimante par défaut.

```csharp
public byte[] PrinterSettings { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrinterSettingsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Test Printer Settings");
            
            // Accéder à la configuration de la page
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Définir les paramètres de l'imprimante (en tableau d'octets)
            byte[] printerSettings = new byte[10]; // Simplified example
            pageSetup.PrinterSettings = printerSettings;
            
            // Vérifiez que les paramètres de l'imprimante sont définis
            Console.WriteLine("Printer Settings: " + (pageSetup.PrinterSettings != null));
            
            // Enregistrez le classeur
            workbook.Save("PrinterSettingsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


