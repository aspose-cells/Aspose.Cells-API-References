---
title: "PowerQueryFormula.Description"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PowerQueryFormula özelliği. Power query formülünün açıklamasını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.querytables/powerqueryformula/description/
---
## PowerQueryFormula.Description property

Power query formülünün açıklamasını alır ve ayarlar.

```csharp
public string Description { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaPropertyDescriptionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            try
            {
                // Power Query formülleri içeren mevcut bir dosyayı yükle
                workbook = new Workbook("example.xlsx");

                // Mevcut Power Query formüllerine erişin
                if (workbook.DataMashup.PowerQueryFormulas.Count > 0)
                {
                    PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas[0];

                    // Geçerli Description değerini göster
                    Console.WriteLine("Current Description: " + formula.Description);

                    // Yeni bir description ayarla
                    formula.Description = "This is an updated description for the Power Query formula";
                    Console.WriteLine("Updated Description: " + formula.Description);

                    // Çalışma kitabını kaydedin
                    workbook.Save("PowerQueryFormulaDescriptionDemo.xlsx");
                    Console.WriteLine("Description property demonstrated successfully.");
                }
                else
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
                Console.WriteLine("Please ensure the example.xlsx file exists and contains Power Query formulas.");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


