---
title: "IWarningCallback.Warning"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode IWarningCallback. Notre rappel n'a besoin d'implémenter que la méthode Warning"
type: docs
url: /fr/net/aspose.cells/iwarningcallback/warning/
---
## IWarningCallback.Warning method

Notre rappel n'a besoin d'implémenter que la méthode "Warning".

```csharp
public void Warning(WarningInfo warningInfo)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| warningInfo | WarningInfo | info d'avertissement |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IWarningCallbackMethodWarningWithWarningInfoDemo : IWarningCallback
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var demo = new IWarningCallbackMethodWarningWithWarningInfoDemo();
            workbook.Settings.WarningCallback = demo;

            try
            {
                Console.WriteLine("Warning callback is set up. Any warnings during operations will be displayed.");
                
                // Démontrer l'effet en enregistrant avec un scénario d'avertissement potentiel
                worksheet.Cells["A1"].Formula = "=1/0"; // This may trigger a warning
                workbook.Save("WarningDemoOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine($"Warning Type: {warningInfo.Type}");
            Console.WriteLine($"Description: {warningInfo.Description}");
            Console.WriteLine($"Corrected Object: {warningInfo.CorrectedObject ?? "null"}");
        }
    }
}
```

### Voir aussi

* class [WarningInfo](../../warninginfo/)
* interface [IWarningCallback](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


