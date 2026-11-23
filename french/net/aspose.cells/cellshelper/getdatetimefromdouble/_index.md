---
title: "CellsHelper.GetDateTimeFromDouble"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CellsHelper. Convertit la valeur double en valeur date‑heure"
type: docs
url: /fr/net/aspose.cells/cellshelper/getdatetimefromdouble/
---
## CellsHelper.GetDateTimeFromDouble method

Convertit la valeur double en valeur date‑heure.

```csharp
public static DateTime GetDateTimeFromDouble(double doubleValue, bool date1904)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| doubleValue | Double | La valeur double. |
| date1904 | Boolean | Système de date 1904. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodGetDateTimeFromDoubleWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Préparez les données pour les paramètres de la méthode (Double, Boolean)
            double doubleValue = 44197.5; // Represents 2021-01-01 12:00:00 in Excel serial date format
            bool date1904 = false; // Using 1900 date system

            try
            {
                // Appelez la méthode GetDateTimeFromDouble avec les types de paramètres spécifiques
                DateTime result = CellsHelper.GetDateTimeFromDouble(doubleValue, date1904);
                
                // Afficher le résultat
                Console.WriteLine($"Converted DateTime: {result}");
                
                // Écrivez le résultat dans une cellule
                worksheet.Cells["A1"].PutValue("Original Double Value:");
                worksheet.Cells["B1"].PutValue(doubleValue);
                worksheet.Cells["A2"].PutValue("Converted DateTime:");
                worksheet.Cells["B2"].PutValue(result.ToString());
                
                Console.WriteLine("Method executed successfully with parameters (Double, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDateTimeFromDouble method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("MethodGetDateTimeFromDoubleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


