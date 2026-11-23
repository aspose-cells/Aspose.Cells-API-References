---
title: "ProtectedRange.AddArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ProtectedRange. Ajoute une zone référencée à celle-ci"
type: docs
url: /fr/net/aspose.cells/protectedrange/addarea/
---
## ProtectedRange.AddArea method

Ajoute une zone référencée à celle-ci

```csharp
public void AddArea(int startRow, int startColumn, int endRow, int endColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | La ligne de départ. |
| startColumn | Int32 | La colonne de départ. |
| endRow | Int32 | La ligne de fin. |
| endColumn | Int32 | La colonne de fin. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectedRangeMethodAddAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add renvoie l'index du nouveau ProtectedRange dans la collection
            int protectedRangeIndex = worksheet.AllowEditRanges.Add("DemoProtectedRange", 0, 0, 0, 0);
            ProtectedRange protectedRange = worksheet.AllowEditRanges[protectedRangeIndex];

            try
            {
                protectedRange.AddArea(2, 2, 5, 5);
                Console.WriteLine("Added new area to protected range.");

                CellArea[] areas = protectedRange.GetAreas();
                Console.WriteLine($"Total protected areas: {areas.Length}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            worksheet.Protect(ProtectionType.All, "password123", null);
            workbook.Save("ProtectedRangeAddAreaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


