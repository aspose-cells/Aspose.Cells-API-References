---
title: "Protection.AllowUsingPivotTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Protection. Rappresenta se l'utente è autorizzato a manipolare le tabelle pivot su un foglio di lavoro protetto"
type: docs
url: /it/net/aspose.cells/protection/allowusingpivottable/
---
## Protection.AllowUsingPivotTable property

Rappresenta se all'utente è consentito manipolare le tabelle pivot su un foglio di lavoro protetto.

```csharp
public bool AllowUsingPivotTable { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowUsingPivotTableDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Abilita la protezione del foglio di lavoro
            Protection protection = worksheet.Protection;
            protection.AllowUsingPivotTable = true;
            worksheet.Protect(ProtectionType.All);

            // Verifica l'impostazione
            Console.WriteLine("AllowUsingPivotTable is set to: " + protection.AllowUsingPivotTable);

            // Crea una tabella pivot per dimostrare la funzionalità
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);

            // Crea una tabella pivot con i parametri corretti
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "C1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Salva la cartella di lavoro
            workbook.Save("ProtectionPropertyAllowUsingPivotTableDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


