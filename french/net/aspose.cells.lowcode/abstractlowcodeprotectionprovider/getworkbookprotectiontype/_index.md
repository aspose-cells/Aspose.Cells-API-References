---
title: "AbstractLowCodeProtectionProvider.GetWorkbookProtectionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AbstractLowCodeProtectionProvider. Obtient le type de protection pour protéger le classeur"
type: docs
url: /fr/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworkbookprotectiontype/
---
## AbstractLowCodeProtectionProvider.GetWorkbookProtectionType method

Obtient le type de protection pour protéger le classeur.

```csharp
public virtual ProtectionType GetWorkbookProtectionType()
```

### Valeur de retour

Type de protection pour protéger le classeur. Aucun signifie aucune protection pour le classeur.

### Exemples

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

### Voir aussi

* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


