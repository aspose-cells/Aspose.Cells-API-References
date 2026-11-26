---
title: "AbstractLowCodeProtectionProvider.GetWorkbookProtectionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AbstractLowCodeProtectionProvider. Obtiene el tipo de protección para proteger el libro de trabajo"
type: docs
url: /es/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookprotectiontype/
---
## AbstractLowCodeProtectionProvider.GetWorkbookProtectionType method

Obtiene el tipo de protección para proteger el libro de trabajo.

```csharp
public virtual ProtectionType GetWorkbookProtectionType()
```

### Valor de retorno

Tipo de protección para proteger el libro de trabajo. Ninguno significa que no hay protección para el libro de trabajo.

### Ejemplos

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

### Ver también

* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


