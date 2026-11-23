---
title: "AbstractLowCodeProtectionProvider.GetWorkbookPassword"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AbstractLowCodeProtectionProvider. Obtient le mot de passe pour protéger le classeur avec le type de protection spécifié"
type: docs
url: /fr/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookpassword/
---
## AbstractLowCodeProtectionProvider.GetWorkbookPassword method

Obtient le mot de passe pour protéger le classeur avec le type de protection spécifié.

```csharp
public virtual string GetWorkbookPassword()
```

### Valeur de retour

Mot de passe pour protéger le classeur.

### Exemples

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

### Voir aussi

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


