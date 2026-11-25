---
title: "Metered.IsMeteredLicensed"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Metered. Verifica se metered è licenziato"
type: docs
url: /it/net/aspose.cells/metered/ismeteredlicensed/
---
## Metered.IsMeteredLicensed method

Verifica se Metered è licenziato

```csharp
public static bool IsMeteredLicensed()
```

### Valore di ritorno

Vero o falso

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodIsMeteredLicensedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza Metered
            Metered metered = new Metered();

            try
            {
                // Verifica se la licenza metered è applicata
                bool isLicensed = Metered.IsMeteredLicensed();

                // Visualizza il risultato
                Console.WriteLine($"Is Metered Licensed: {isLicensed}");

                // Aggiungi il risultato al foglio di lavoro
                worksheet.Cells["A1"].PutValue("Is Metered Licensed:");
                worksheet.Cells["B1"].PutValue(isLicensed);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsMeteredLicensed method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("MethodIsMeteredLicensedDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


