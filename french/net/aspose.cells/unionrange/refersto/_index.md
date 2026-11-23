---
title: "UnionRange.RefersTo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété UnionRange. Obtient les plages auxquelles il fait référence"
type: docs
url: /fr/net/aspose.cells/unionrange/refersto/
---
## UnionRange.RefersTo property

Obtient la référence de la plage.

```csharp
public string RefersTo { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyRefersToDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplissez quelques données
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(800);

            // Créer une plage nommée
            Aspose.Cells.Range namedRange = worksheet.Cells.CreateRange("B2:B3");
            namedRange.Name = "ProductPrices";

            // Créer une plage d'union qui inclut notre plage nommée
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B3").UnionRanges(new Aspose.Cells.Range[] { namedRange });

            // Afficher la propriété RefersTo de la plage d'union
            Console.WriteLine("UnionRange RefersTo: " + unionRange.RefersTo);

            // Créer une autre plage et afficher son RefersTo
            Aspose.Cells.Range singleRange = worksheet.Cells.CreateRange("C1:D3");
            Console.WriteLine("Single Range RefersTo: " + singleRange.RefersTo);

            // Démontrer l'utilisation de RefersTo pour identifier la composition de la plage
            Console.WriteLine("Does union range contain named range? " + 
                unionRange.RefersTo.Contains("ProductPrices"));

            // Montrer comment RefersTo change lorsque les plages sont modifiées
            Aspose.Cells.Range newRange = worksheet.Cells.CreateRange("A1:C3");
            UnionRange modifiedUnion = newRange.UnionRanges(new Aspose.Cells.Range[] { namedRange });
            Console.WriteLine("Modified UnionRange RefersTo: " + modifiedUnion.RefersTo);

            // Enregistrez le classeur
            workbook.Save("UnionRangeRefersToDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


