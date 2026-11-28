---
title: "PowerQueryFormulaItemCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PowerQueryFormulaItemCollection özelliği. Listedeki indekse göre PowerQueryFormulaItem alır"
type: docs
url: /tr/net/aspose.cells.querytables/powerqueryformulaitemcollection/item/
---
## PowerQueryFormulaItemCollection indexer (1 of 2)

Listedeki indekse göre [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) alır.

```csharp
public PowerQueryFormulaItem this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaItemCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Power Query içeren bir şablonla yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk Power Query formülünü al (var olduğunu varsayarak)
            var powerQueryFormula = workbook.DataMashup.PowerQueryFormulas[0];
            
            // Item özelliğini kullanarak formül öğelerini değiştir
            var formulaItems = powerQueryFormula.PowerQueryFormulaItems;
            if (formulaItems.Count > 0)
            {
                formulaItems[0].Value = "Sql.Database(\"SQL2K16\", \"EUC876REG\", [Query=\"select * from CANOTIFICATIONS\"])";
                
                // Değişikliği doğrulayın
                Console.WriteLine(formulaItems[0].Value);
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("PowerQueryExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)

---

## PowerQueryFormulaItemCollection indexer (2 of 2)

Öğenin adına göre [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) alır.

```csharp
public PowerQueryFormulaItem this[string name] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| name | Öğenin adı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaItemCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            try
            {
                // Power Query formüllerini içeren bir çalışma kitabını yükle.
                // Yolun yerine, mevcutsa Power Query içeren gerçek bir dosya koy.
                string sourcePath = "PowerQuerySample.xlsx";
                Workbook workbook = System.IO.File.Exists(sourcePath) ? new Workbook(sourcePath) : new Workbook();

                // Power Query formüllerinin koleksiyonuna eriş.
                PowerQueryFormulaCollection pqFormulas = workbook.DataMashup.PowerQueryFormulas;

                if (pqFormulas.Count == 0)
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                    return;
                }

                // İlk Power Query formülünü al.
                PowerQueryFormula formula = pqFormulas[0];

                // Öğeler koleksiyonuna eriş.
                PowerQueryFormulaItemCollection items = formula.PowerQueryFormulaItems;

                if (items.Count == 0)
                {
                    Console.WriteLine("The selected Power Query formula contains no items.");
                    return;
                }

                // Geçerli bir öğe adı elde etmek için ilk öğeyi al.
                PowerQueryFormulaItem firstItem = items[0];
                string itemName = firstItem.Name;

                // Aynı öğeyi adına göre almak için Item(string) indeksleyicisini (yalnızca okuma) kullan.
                PowerQueryFormulaItem retrievedItem = items[itemName];

                // Alınan öğenin özelliklerini göster.
                Console.WriteLine($"Item Name : {retrievedItem.Name}");
                Console.WriteLine($"Item Value: {retrievedItem.Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


