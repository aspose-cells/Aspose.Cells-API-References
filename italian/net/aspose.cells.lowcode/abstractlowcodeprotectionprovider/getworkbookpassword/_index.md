---
title: "AbstractLowCodeProtectionProvider.GetWorkbookPassword"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AbstractLowCodeProtectionProvider. Ottiene la password per proteggere il workbook con il tipo di protezione specificato"
type: docs
url: /it/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookpassword/
---
## AbstractLowCodeProtectionProvider.GetWorkbookPassword method

Ottiene la password per proteggere la cartella di lavoro con il tipo di protezione specificato.

```csharp
public virtual string GetWorkbookPassword()
```

### Valore di ritorno

Password per proteggere il workbook.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWorkbookPasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var provider = new DemoProtectionProvider();

            try
            {
                string password = provider.GetWorkbookPassword();
                ProtectionType protectionType = provider.GetWorkbookProtectionType();

                workbook.Protect(protectionType, password);
                Console.WriteLine($"Workbook protected with password: {password}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ProtectedWorkbook.xlsx");

        }
    }

    public class DemoProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetWorkbookPassword()
        {
            return "Aspose1234!";
        }

        public override ProtectionType GetWorkbookProtectionType()
        {
            return ProtectionType.Structure;
        }
        
    }
}
```

### Vedi anche

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


