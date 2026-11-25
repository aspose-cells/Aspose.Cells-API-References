---
title: "AbstractLowCodeProtectionProvider.GetWritePassword"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AbstractLowCodeProtectionProvider. Ottiene la password per modificare il file del foglio di calcolo"
type: docs
url: /it/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getwritepassword/
---
## AbstractLowCodeProtectionProvider.GetWritePassword method

Ottiene la password per modificare il file di foglio di calcolo.

```csharp
public virtual string GetWritePassword()
```

### Valore di ritorno

Password per modificare il file del foglio di calcolo. Vuoto indica nessuna protezione per la modifica del file.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWritePasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Crea un'istanza del provider di protezione personalizzato
            var protectionProvider = new CustomProtectionProvider();

            try
            {
                // Chiama esplicitamente GetWritePassword e visualizza il risultato
                string writePassword = protectionProvider.GetWritePassword();
                Console.WriteLine($"Retrieved write password: {writePassword}");

                // Salva il workbook - applica direttamente la protezione di scrittura
                workbook.Settings.WriteProtection.Password = writePassword;
                workbook.Save("MethodGetWritePasswordDemo.xlsx");
                Console.WriteLine("Workbook saved with write protection password.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetWritePassword method: {ex.Message}");
            }
        }

    }

    // Implementazione del provider di protezione personalizzato
    public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetWritePassword()
        {
            return "AsposeTestPassword123!";
        }

        // Implementa gli altri metodi richiesti con valori di ritorno predefiniti
        public override string GetOpenPassword() => null;
        public override string GetWorkbookPassword() => null;
        public override ProtectionType GetWorkbookProtectionType() => ProtectionType.None;
        public override string GetWorksheetPassword(string sheetName) => null;
        public override ProtectionType GetWorksheetProtectionType(string sheetName) => ProtectionType.None;
    }
}
```

### Vedi anche

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


