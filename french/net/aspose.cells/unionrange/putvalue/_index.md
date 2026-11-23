---
title: "UnionRange.PutValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode UnionRange. Insère une valeur dans la plage ; si approprié, la valeur sera convertie en un autre type de données et le format numérique des cellules sera réinitialisé"
type: docs
url: /fr/net/aspose.cells/unionrange/putvalue/
---
## UnionRange.PutValue method

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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créez une plage d'union couvrant les cellules A1 à B2
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });
            
            try
            {
                // Appeler PutValue avec les paramètres : (String, Boolean, Boolean)
                unionRange.PutValue("Sample Value", true, true);
                
                Console.WriteLine("PutValue method executed successfully with parameters (String, Boolean, Boolean)");
                
                // Afficher les informations de la plage pour montrer l'effet
                Console.WriteLine($"Range address: {unionRange.RefersTo}");
                Console.WriteLine($"Value set in range: {unionRange.Value}");
                
                // Appliquer le formatage pour rendre l'effet visible
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                style.HorizontalAlignment = TextAlignmentType.Center;
                unionRange.SetStyle(style);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PutValue method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("UnionRangeMethodPutValueWithStringBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


