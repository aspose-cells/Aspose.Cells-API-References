---
title: "AbstractLowCodeProtectionProvider.GetOpenPassword"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AbstractLowCodeProtectionProvider. Ottiene la password per aprire il file di foglio di calcolo"
type: docs
url: /it/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getopenpassword/
---
## AbstractLowCodeProtectionProvider.GetOpenPassword method

Ottiene la password per aprire il file di foglio di calcolo.

```csharp
public virtual string GetOpenPassword()
```

### Valore di ritorno

Password per aprire il file di foglio di calcolo. Vuoto indica nessuna protezione per l'apertura del file.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetOpenPasswordDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un'istanza del provider di protezione
                var protectionProvider = new DemoProtectionProvider();

                // Chiama il metodo GetOpenPassword per recuperare la password
                string password = protectionProvider.GetOpenPassword();

                // Crea un nuovo workbook e applica la password
                Workbook workbook = new Workbook("sample.xlsx");
                workbook.Settings.Password = password;

                // Salva il workbook protetto da password
                workbook.Save("MethodGetOpenPasswordDemo.xlsx");

                Console.WriteLine($"Workbook protected with open password: {password}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing demo: {ex.Message}");
            }
        }
    }

    public class DemoProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetOpenPassword()
        {
            return "AsposeDemo123!";
        }
    }
}
```

### Vedi anche

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


