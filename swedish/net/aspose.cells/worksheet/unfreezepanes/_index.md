---
title: "Worksheet.UnFreezePanes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Avfryser rutor i worksheet"
type: docs
url: /sv/net/aspose.cells/worksheet/unfreezepanes/
---
## Worksheet.UnFreezePanes method

Låser upp fönstren i kalkylbladet.

```csharp
public void UnFreezePanes()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodUnFreezePanesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Frys rutor vid cell C3 (rader 2, kolumner 2 frysta)
            worksheet.FreezePanes("C3", 2, 2);

            // Verifiera att rutor är frysta
            int frozenRow, frozenColumn, frozenRows, frozenColumns;
            worksheet.GetFreezedPanes(out frozenRow, out frozenColumn, out frozenRows, out frozenColumns);
            Console.WriteLine($"Frozen panes - Row: {frozenRow}, Column: {frozenColumn}, Rows: {frozenRows}, Columns: {frozenColumns}");

            // Avfrys rutorna
            worksheet.UnFreezePanes();

            // Verifiera att rutor är avfrysta
            worksheet.GetFreezedPanes(out frozenRow, out frozenColumn, out frozenRows, out frozenColumns);
            Console.WriteLine($"After UnFreezePanes - Row: {frozenRow}, Column: {frozenColumn}, Rows: {frozenRows}, Columns: {frozenColumns}");

            // Spara arbetsboken
            workbook.Save("UnFreezePanesDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


