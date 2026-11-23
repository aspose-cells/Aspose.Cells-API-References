---
title: "ProtectedRange.IsProtectedWithPassword"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ProtectedRange property. Indique si la feuille de calcul est protégée par un mot de passe"
type: docs
url: /fr/net/aspose.cells/protectedrange/isprotectedwithpassword/
---
## ProtectedRange.IsProtectedWithPassword property

Indique si la feuille de calcul est protégée par un mot de passe.

```csharp
public bool IsProtectedWithPassword { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyIsProtectedWithPasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer des plages protégées et obtenir leurs indices
            int protectedIndex = worksheet.AllowEditRanges.Add("PasswordProtected", 0, 0, 5, 5);
            ProtectedRange protectedWithPassword = worksheet.AllowEditRanges[protectedIndex];
            protectedWithPassword.Password = "test123";
            
            int unprotectedIndex = worksheet.AllowEditRanges.Add("Unprotected", 6, 0, 11, 5);
            ProtectedRange unprotected = worksheet.AllowEditRanges[unprotectedIndex];
            
            // Protéger la feuille de calcul pour appliquer des restrictions
            worksheet.Protect(ProtectionType.All);
            
            // Vérifier l'état de la protection par mot de passe
            Console.WriteLine($"Range '{protectedWithPassword.Name}' password protected: {protectedWithPassword.IsProtectedWithPassword}");
            Console.WriteLine($"Range '{unprotected.Name}' password protected: {unprotected.IsProtectedWithPassword}");
        }
    }
}
```

### Voir aussi

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


