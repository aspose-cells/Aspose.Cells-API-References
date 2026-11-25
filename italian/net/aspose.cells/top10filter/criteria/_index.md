---
title: "Top10Filter.Criteria"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Top10Filter. Il valore reale della cella nell'intervallo utilizzato per eseguire il confronto per questo filtro. Questo è il valore di cache durante il processo di aggiornamento"
type: docs
url: /it/net/aspose.cells/top10filter/criteria/
---
## Top10Filter.Criteria property

Il valore reale della cella nell'intervallo utilizzato per eseguire il confronto per questo filtro. Questo è il valore di cache durante il processo di aggiornamento.

```csharp
[Obsolete("Ignore this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public object Criteria { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di ignorare questa proprietà. Questa proprietà sarà rimossa tra 12 mesi a partire da ottobre 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class Top10FilterPropertyCriteriaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            for (int i = 0; i < 20; i++)
            {
                worksheet.Cells[i, 0].PutValue(20 - i);
            }
            
            worksheet.AutoFilter.Range = "A1:A20";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5);
            
            // Correzione: Accedi alla proprietà Filter e cast a Top10Filter
            Top10Filter filter = (Top10Filter)worksheet.AutoFilter.FilterColumns[0].Filter;
            Console.WriteLine("Current Criteria value: " + filter.Criteria);
            
            filter.Criteria = 14;
            
            worksheet.AutoFilter.Refresh();
            
            workbook.Save("Top10FilterCriteriaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


