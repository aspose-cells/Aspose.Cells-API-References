---
title: "AbstractLowCodeProtectionProvider.GetWorksheetPassword"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AbstractLowCodeProtectionProvider. Ottiene la password per proteggere il foglio di lavoro specificato"
type: docs
url: /it/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetpassword/
---
## AbstractLowCodeProtectionProvider.GetWorksheetPassword method

Ottiene la password per proteggere il foglio di lavoro specificato.

```csharp
public virtual string GetWorksheetPassword(string sheetName)
```

### Valore di ritorno

Password per proteggere il foglio di lavoro specificato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWorksheetPasswordWithStringDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            string sheetName = worksheet.Name;

            // Crea un'istanza del provider di protezione personalizzato
            var provider = new CustomProtectionProvider();

            try
            {
                // Chiama GetWorksheetPassword con il nome del foglio di lavoro
                string password = provider.GetWorksheetPassword(sheetName);

                // Applica la protezione al foglio di lavoro usando la password recuperata
                worksheet.Protect(ProtectionType.All, password, null);

                Console.WriteLine($"Protected worksheet '{sheetName}' with password: {password}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetWorksheetPassword: {ex.Message}");
            }

            // Salva la cartella di lavoro protetta
            workbook.Save("WorksheetPasswordDemo.xlsx");

        }
    }

    // Implementazione personalizzata che restituisce la password basata sul nome del foglio
    public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public new string GetWorksheetPassword(string sheetName)
        {
            // Logica semplice di generazione della password per dimostrazione
            return $"pw_{sheetName}";
        }
    }
}
```

### Vedi anche

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


