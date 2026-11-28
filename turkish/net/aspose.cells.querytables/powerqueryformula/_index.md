---
title: "Sınıf PowerQueryFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.QueryTables.PowerQueryFormula sınıfı. Power query formülünün tanımını temsil eder"
type: docs
url: /tr/net/aspose.cells.querytables/powerqueryformula/
---
## PowerQueryFormula class

Power Query formülünün tanımını temsil eder.

```csharp
public class PowerQueryFormula
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Power query formülünün açıklamasını alır ve ayarlar. |
| virtual [FormulaDefinition](../../aspose.cells.querytables/powerqueryformula/formuladefinition/) { get; } | Power query formülünün tanımını alır. |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Bu power query formülünü içeren grup adını alır. |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Power query formülünün adını alır ve ayarlar. |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Power query formülünün tüm öğelerini alır. |
| virtual [Type](../../aspose.cells.querytables/powerqueryformula/type/) { get; } | Bu power query formülünün tipini alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class QueryTablesClassPowerQueryFormulaDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // DataMashup'tan PowerQueryFormulas koleksiyonuna erişin
                PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;

                // Mevcut formüllerin olup olmadığını kontrol edin
                if (formulas.Count > 0)
                {
                    // İlk PowerQueryFormula'yı alın
                    PowerQueryFormula formula = formulas[0];

                    // Yalnızca okunabilir özellikleri göster
                    Console.WriteLine($"Formula Type: {formula.Type}");
                    Console.WriteLine($"Group Name: {formula.GroupName}");
                    Console.WriteLine($"Formula Definition: {formula.FormulaDefinition}");

                    // Okuma-yazma özelliklerini görüntüleyin ve değiştirin
                    Console.WriteLine($"Original Name: {formula.Name}");
                    formula.Name = "ModifiedFormulaName";
                    Console.WriteLine($"Modified Name: {formula.Name}");

                    Console.WriteLine($"Original Description: {formula.Description}");
                    formula.Description = "Updated description for the formula";
                    Console.WriteLine($"Modified Description: {formula.Description}");

                    // Formül öğelerinin sayısını görüntüleyin
                    Console.WriteLine($"Number of Formula Items: {formula.PowerQueryFormulaItems.Count}");
                }
                else
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                    Console.WriteLine("This is expected for a new workbook.");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("PowerQueryFormulaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PowerQueryFormula: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


