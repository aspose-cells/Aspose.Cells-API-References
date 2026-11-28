---
title: "Sınıf PowerQueryFormulaItem"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.QueryTables.PowerQueryFormulaItem sınıfı. Power query formülünün öğesini temsil eder"
type: docs
url: /tr/net/aspose.cells.querytables/powerqueryformulaitem/
---
## PowerQueryFormulaItem class

Power Query formülünün öğesini temsil eder.

```csharp
public class PowerQueryFormulaItem
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ItemType](../../aspose.cells.querytables/powerqueryformulaitem/itemtype/) { get; } | Bu öğenin tipini alır (Function, Parameter, List, Literal veya Unknown). |
| [Name](../../aspose.cells.querytables/powerqueryformulaitem/name/) { get; } | Öğenin adını alır. |
| [TextValue](../../aspose.cells.querytables/powerqueryformulaitem/textvalue/) { get; } | Öğenin metin değerini alır. |
| [Value](../../aspose.cells.querytables/powerqueryformulaitem/value/) { get; set; } | Öğenin değerini alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;

    public class QueryTablesClassPowerQueryFormulaItemDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluşturun (Power Query veriniz varsa mevcut bir dosya da olabilir)
                Workbook workbook = new Workbook();

                // PowerQuery formüllerini içeren DataMashup nesnesine erişin
                DataMashup mashup = workbook.DataMashup;

                bool itemFound = false;

                // Tüm PowerQuery formüllerini ve öğelerini yineleyin
                foreach (PowerQueryFormula formula in mashup.PowerQueryFormulas)
                {
                    foreach (PowerQueryFormulaItem item in formula.PowerQueryFormulaItems)
                    {
                        // Salt okunur Name özelliğini gösterin
                        Console.WriteLine($"Item Name: {item.Name}");

                        // Okuma/yazma Value özelliğini gösterin
                        Console.WriteLine($"Original Value: {item.Value}");
                        item.Value = "SampleValue";
                        Console.WriteLine($"Modified Value: {item.Value}");

                        itemFound = true;
                    }
                }

                if (!itemFound)
                {
                    Console.WriteLine("No PowerQueryFormulaItem instances were found in the workbook.");
                }

                Console.WriteLine("PowerQueryFormulaItem demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PowerQueryFormulaItem: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


