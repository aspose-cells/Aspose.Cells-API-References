---
title: "WorksheetCollection.OleSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-egenskap. Hämtar och anger den visade storleken när Workbook-filen används som ett Ole-objekt"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/olesize/
---
## WorksheetCollection.OleSize property

Hämtar och anger visad storlek när Workbook-filen används som ett Ole-objekt.

```csharp
public object OleSize { get; set; }
```

### Anmärkningar

Null betyder ingen ole-storleksinställning.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyOleSizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ange OLE-storleken för arbetsbladssamlingen
            workbook.Worksheets.SetOleSize(0, 10, 0, 10);
            
            // Kom åt och visa OLE-storleks-egenskaperna
            CellArea oleSize = (CellArea)workbook.Worksheets.OleSize;
            Console.WriteLine("OLE Size Range:");
            Console.WriteLine($"StartRow: {oleSize.StartRow}, EndRow: {oleSize.EndRow}");
            Console.WriteLine($"StartColumn: {oleSize.StartColumn}, EndColumn: {oleSize.EndColumn}");
            
            // Spara arbetsboken
            workbook.Save("OleSizeDemo.xlsx");
        }
    }
}
```

### Se även

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


