---
title: "Hyperlink.Delete"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Hyperlink. Supprime ce lien hypertexte."
type: docs
url: /fr/net/aspose.cells/hyperlink/delete/
---
## Hyperlink.Delete method

Supprime ce lien hypertexte

```csharp
public void Delete()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkMethodDeleteDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez quelques liens hypertexte pour démontrer la suppression
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            worksheet.Hyperlinks.Add("B2", 1, 1, "https://www.example.com");
            
            Console.WriteLine($"Hyperlinks count before deletion: {worksheet.Hyperlinks.Count}");
            
            // Supprimez tous les liens hypertexte
            for (int i = worksheet.Hyperlinks.Count - 1; i >= 0; i--)
            {
                worksheet.Hyperlinks[i].Delete();
            }
            
            Console.WriteLine($"Hyperlinks count after deletion: {worksheet.Hyperlinks.Count}");
        }
    }
}
```

### Voir aussi

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


