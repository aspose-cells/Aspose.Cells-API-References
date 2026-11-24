---
title: "TableStyleCollection.DefaultPivotStyleName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TableStyleCollection-Eigenschaft. Liest und schreibt den Standardstilnamen der Pivot-Tabelle"
type: docs
url: /de/net/aspose.cells.tables/tablestylecollection/defaultpivotstylename/
---
## TableStyleCollection.DefaultPivotStyleName property

Liest und setzt den Standardstilnamen der Pivot-Tabelle.

```csharp
public string DefaultPivotStyleName { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleCollectionPropertyDefaultPivotStyleNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf die Sammlung der Tabellestile zu
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            
            // Standard-Pivot-Stilnamen anzeigen
            Console.WriteLine("Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
            
            // Standard-Pivot-Stil ändern
            tableStyles.DefaultPivotStyleName = "PivotStyleDark2";
            
            // Die Änderung überprüfen
            Console.WriteLine("Updated Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


