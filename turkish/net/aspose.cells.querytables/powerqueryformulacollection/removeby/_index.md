---
title: "PowerQueryFormulaCollection.RemoveBy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PowerQueryFormulaCollection yöntemi. Power Query formülünü ad ile kaldır"
type: docs
url: /tr/net/aspose.cells.querytables/powerqueryformulacollection/removeby/
---
## PowerQueryFormulaCollection.RemoveBy method

Power query formülünü ad ile kaldır.

```csharp
public void RemoveBy(string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Power Query formülünün adı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaCollectionMethodRemoveByWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // PowerQueryFormulaCollection'a erişin (çalışma kitabında mevcut olduğunu varsayarak)
                PowerQueryFormulaCollection powerQueryFormulas = workbook.DataMashup.PowerQueryFormulas;
                
                // Kaldırılacak örnek bir formül ekleyin (bu genellikle mevcut verilerden gelir)
                string formulaName = "SampleFormula";
                
                // Formül adıyla RemoveBy'yi çağırın
                powerQueryFormulas.RemoveBy(formulaName);
                
                Console.WriteLine($"Formula '{formulaName}' removed successfully");
                
                // Çalışma kitabını kaydedin
                workbook.Save("RemoveByWithStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in RemoveBy demonstration: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


