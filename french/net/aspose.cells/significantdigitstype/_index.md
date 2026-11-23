---
title: "Enum SignificantDigitsType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.SignificantDigitsType enum. Représente le type de chiffres significatifs pour la sortie des valeurs numériques"
type: docs
url: /fr/net/aspose.cells/significantdigitstype/
---
## SignificantDigitsType enumeration

Représente le type de chiffres significatifs pour la sortie des valeurs numériques.

```csharp
public enum SignificantDigitsType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Digits15 | `0` | 15-chiffres |
| G17 | `1` | 17-chiffres en formatant la valeur avec "G17". |
| Rounding17 | `2` | 17-chiffres en arrondissant la valeur. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassSignificantDigitsTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Créez un nouveau classeur pour la démonstration
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Démontrez l'utilisation de chaque valeur de l'énumération SignificantDigitsType
                SignificantDigitsType[] types = {
                    SignificantDigitsType.Digits15,
                    SignificantDigitsType.G17,
                    SignificantDigitsType.Rounding17
                };

                foreach (SignificantDigitsType type in types)
                {
                    // Définissez le type de chiffres significatifs pour le classeur
                    workbook.Settings.SignificantDigitsType = type;

                    // Affichez le paramètre actuel
                    Console.WriteLine($"Current SignificantDigitsType: {type} (Value: {(int)type})");

                    // Ajoutez une valeur d'exemple pour démontrer le paramètre
                    worksheet.Cells["A1"].PutValue(123.4567890123456789);

                    // Enregistrez le classeur avec le paramètre actuel
                    string fileName = $"SignificantDigitsType_{type}.xlsx";
                    workbook.Save(fileName);
                    Console.WriteLine($"Workbook saved with {type} setting as {fileName}");
                }

                Console.WriteLine("All SignificantDigitsType demonstrations completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating SignificantDigitsType: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


