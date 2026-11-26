---
title: "AbstractLowCodeProtectionProvider.GetWorkbookPassword"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AbstractLowCodeProtectionProvider. Obtiene la contraseña para proteger el libro de trabajo con el tipo de protección especificado"
type: docs
url: /es/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookpassword/
---
## AbstractLowCodeProtectionProvider.GetWorkbookPassword method

Obtiene la contraseña para proteger el libro de trabajo con el tipo de protección especificado.

```csharp
public virtual string GetWorkbookPassword()
```

### Valor de retorno

Contraseña para proteger el libro de trabajo.

### Ejemplos

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

### Ver también

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


