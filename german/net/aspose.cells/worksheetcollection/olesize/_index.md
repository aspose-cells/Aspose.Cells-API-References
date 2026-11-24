---
title: "WorksheetCollection.OleSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Eigenschaft. Liest und setzt die angezeigte Größe, wenn die Workbook-Datei als Ole-Objekt verwendet wird."
type: docs
url: /de/net/aspose.cells/worksheetcollection/olesize/
---
## WorksheetCollection.OleSize property

Ruft die angezeigte Größe ab und legt sie fest, wenn die Arbeitsmappendatei als Ole‑Objekt verwendet wird.

```csharp
public object OleSize { get; set; }
```

### Hinweise

Null bedeutet, dass keine Ole-Größeneinstellung vorhanden ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyOleSizeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Setze die OLE-Größe für die WorksheetCollection.
            workbook.Worksheets.SetOleSize(0, 10, 0, 10);
            
            // Greife auf die OLE-Größeneigenschaften zu und zeige sie an.
            CellArea oleSize = (CellArea)workbook.Worksheets.OleSize;
            Console.WriteLine("OLE Size Range:");
            Console.WriteLine($"StartRow: {oleSize.StartRow}, EndRow: {oleSize.EndRow}");
            Console.WriteLine($"StartColumn: {oleSize.StartColumn}, EndColumn: {oleSize.EndColumn}");
            
            // Speichere die Arbeitsmappe
            workbook.Save("OleSizeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


