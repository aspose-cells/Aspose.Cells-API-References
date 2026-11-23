---
title: "Cell.StringValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cell. Obtient la valeur chaîne contenue dans la cellule. Si le type de cette cellule est string, alors renvoie la valeur chaîne elle-même. Pour les autres types de cellules, la valeur chaîne formatée selon le style spécifié de cette cellule sera renvoyée. La valeur de cellule formatée est identique à ce que vous pouvez obtenir depuis Excel en copiant une cellule en tant que texte, comme copier la cellule vers un éditeur de texte ou exporter en csv"
type: docs
url: /fr/net/aspose.cells/cell/stringvalue/
---
## Cell.StringValue property

Obtient la valeur chaîne contenue dans la cellule. Si le type de cette cellule est chaîne, la valeur chaîne elle‑même est retournée. Pour les autres types de cellules, la valeur chaîne formatée (formatée avec le style spécifié de cette cellule) est retournée. La valeur de cellule formatée est identique à ce que vous pouvez obtenir depuis Excel en copiant une cellule en tant que texte (par exemple en copiant la cellule dans un éditeur de texte ou en l'exportant vers CSV).

```csharp
public string StringValue { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyStringValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir certaines valeurs
            cells["A1"].PutValue("Hello");
            cells["A2"].PutValue(123);
            cells["A3"].PutValue(DateTime.Now);
            cells["A4"].Formula = "=A1&A2";

            // Calculer les formules
            workbook.CalculateFormula();

            // Démontrer la propriété StringValue
            Console.WriteLine("A1 StringValue: " + cells["A1"].StringValue);
            Console.WriteLine("A2 StringValue: " + cells["A2"].StringValue);
            Console.WriteLine("A3 StringValue: " + cells["A3"].StringValue);
            Console.WriteLine("A4 StringValue: " + cells["A4"].StringValue);

            // Afficher le cas de valeur d'erreur
            Cell errorCell = cells["B1"];
            errorCell.Formula = "=1/0";
            workbook.CalculateFormula();
            Console.WriteLine("B1 (Error) StringValue: " + errorCell.StringValue);
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


