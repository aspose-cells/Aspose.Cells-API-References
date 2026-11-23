---
title: "Protection.AllowSorting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Protection. Indique si l’option de tri est autorisée sur une feuille protégée"
type: docs
url: /fr/net/aspose.cells/protection/allowsorting/
---
## Protection.AllowSorting property

Représente si l'option de tri est autorisée sur une feuille de calcul protégée.

```csharp
public bool AllowSorting { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSortingDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Activer la protection de la feuille
            worksheet.Protect(ProtectionType.All);
            
            // Définir les propriétés de protection incluant AllowSorting
            Protection protection = worksheet.Protection;
            protection.AllowSorting = true;
            protection.AllowFiltering = true;
            protection.AllowEditingContent = false;

            // Afficher les paramètres de protection
            Console.WriteLine("Protection Settings:");
            Console.WriteLine($"AllowSorting: {protection.AllowSorting}");
            Console.WriteLine($"AllowFiltering: {protection.AllowFiltering}");
            Console.WriteLine($"AllowEditingContent: {protection.AllowEditingContent}");

            // Démontrer la capacité de tri
            if (protection.AllowSorting)
            {
                Console.WriteLine("\nSorting is allowed on this protected worksheet");
            }
            else
            {
                Console.WriteLine("\nSorting is not allowed on this protected worksheet");
            }
        }
    }
}
```

### Voir aussi

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


