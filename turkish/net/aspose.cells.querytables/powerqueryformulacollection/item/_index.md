---
title: "PowerQueryFormulaCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PowerQueryFormulaCollection özelliği. Listedeki indekse göre PowerQueryFormula'yi alır"
type: docs
url: /tr/net/aspose.cells.querytables/powerqueryformulacollection/item/
---
## PowerQueryFormulaCollection indexer (1 of 2)

Listedeki indekse göre [`PowerQueryFormula`](../../powerqueryformula/) alır.

```csharp
public PowerQueryFormula this[int index] { get; }
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
    public class PowerQueryFormulaCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Power Query formüllerini al
            var dataMashup = workbook.DataMashup;
            var formulas = dataMashup.PowerQueryFormulas;
            
            // Yeni bir formül oluşturun ve ekleyin (gerekirse)
            // Not: Gerçek uygulama, formülleri eklemek için farklı bir yaklaşım gerektirebilir
            // Demo amaçları için, varsa mevcut formüllerle çalışacağız
            if (formulas.Count == 0)
            {
                // Bu sadece bir gösterim içindir - gerçek API farklı bir yaklaşım gerektirebilir
                // yeni formüller oluşturmak için
                return;
            }

            // Item özelliğini kullanarak ilk formüle erişin
            var formula = formulas[0];
            
            // Formül öğelerini al
            var formulaItems = formula.PowerQueryFormulaItems;
            if (formulaItems.Count == 0)
            {
                // Bu sadece bir gösterim içindir - gerçek API farklı bir yaklaşım gerektirebilir
                // yeni formül öğeleri oluşturmak için
                return;
            }

            // Item özelliğini kullanarak ilk öğeye erişin
            var formulaItem = formulaItems[0];
            
            // Item özelliğini kullanarak değeri ayarlayın ve alın
            string formulaText = "Sql.Database(\"SERVER\", \"DB\", [Query=\"SELECT * FROM TABLE\"])";
            formulaItem.Value = formulaText;
            
            // Item özelliğinin kullanımını göster
            string retrievedValue = formulaItems[0].Value;
            Console.WriteLine("Power Query Formula Item Value: " + retrievedValue);
            
            // Çalışma kitabını kaydedin
            workbook.Save("PowerQueryDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)

---

## PowerQueryFormulaCollection indexer (2 of 2)

Power Query formülünün adına göre [`PowerQueryFormula`](../../powerqueryformula/) alır.

```csharp
public PowerQueryFormula this[string name] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| name | Öğenin adı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Power Query formüllerini içeren mevcut bir dosyayı yükleyerek bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook("example.xlsx");
            
            // Power Query formülleri koleksiyonunu al
            PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Item özelliğinin kullanımını göster
            try
            {
                // Mevcut bir formüle (varsa) erişmeye çalışın
                if (formulas.Count > 0)
                {
                    PowerQueryFormula formula = formulas[formulas[0].Name];
                    Console.WriteLine("First formula found: " + formula.Name);
                    Console.WriteLine("Formula definition: " + formula.FormulaDefinition);
                    Console.WriteLine("Formula type: " + formula.Type);
                }
                
                // Bu, mevcut olmayan formül için bir istisna fırlatacaktır
                PowerQueryFormula nonExistent = formulas["NonExistentFormula"];
            }
            catch (Exception ex)
            {
                Console.WriteLine("Expected error accessing non-existent formula: " + ex.Message);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


