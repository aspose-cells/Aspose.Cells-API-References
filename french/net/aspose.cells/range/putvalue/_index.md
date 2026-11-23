---
title: "Range.PutValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Insère une valeur dans la plage ; si approprié, la valeur sera convertie en un autre type de données et le format numérique des cellules sera réinitialisé"
type: docs
url: /fr/net/aspose.cells/range/putvalue/
---
## Range.PutValue method

Insère une valeur dans la plage, le cas échéant la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stringValue | String | Valeur d'entrée |
| isConverted | Boolean | Vrai: converti en un autre type de données si approprié. |
| setStyle | Boolean | Vrai: définir le format numérique sur le style de la cellule lors de la conversion en un autre type de données |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1:B10");
            range.PutValue("123", true, false);
            
            Console.WriteLine("Value at A5: " + cells["A5"].DoubleValue);
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


