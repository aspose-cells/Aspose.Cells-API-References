---
title: "AbstractLowCodeProtectionProvider.GetWorkbookProtectionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AbstractLowCodeProtectionProvider. Ottiene il tipo di protezione per proteggere il workbook"
type: docs
url: /it/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookprotectiontype/
---
## AbstractLowCodeProtectionProvider.GetWorkbookProtectionType method

Ottiene il tipo di protezione per proteggere la cartella di lavoro.

```csharp
public virtual ProtectionType GetWorkbookProtectionType()
```

### Valore di ritorno

Tipo di protezione per proteggere il workbook. Nessuno indica nessuna protezione per il workbook.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWorkbookProtectionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            var provider = new CustomProtectionProvider();

            try
            {
                workbook.Protect(provider.GetWorkbookProtectionType(), provider.GetWorkbookPassword());
                
                ProtectionType protectionType = provider.GetWorkbookProtectionType();
                Console.WriteLine($"Workbook protection type: {protectionType}");
                Console.WriteLine($"Protection status: {workbook.Settings.IsProtected}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetWorkbookProtectionType: {ex.Message}");
            }

            workbook.Save("WorkbookProtectionDemo.xlsx");
        }


        private class CustomProtectionProvider : AbstractLowCodeProtectionProvider
        {
            public override ProtectionType GetWorkbookProtectionType()
            {
                return ProtectionType.Structure;
            }

            public override string GetWorkbookPassword()
            {
                return "aspose123";
            }
        }
    }
}
```

### Vedi anche

* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


