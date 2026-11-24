---
title: "TableStyleCollection.DefaultTableStyleName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TableStyleCollection-Eigenschaft. Liest und schreibt den Standardstilnamen der Tabelle"
type: docs
url: /de/net/aspose.cells.tables/tablestylecollection/defaulttablestylename/
---
## TableStyleCollection.DefaultTableStyleName property

Liest und setzt den Standardstilnamen der Tabelle.

```csharp
public string DefaultTableStyleName { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleCollectionPropertyDefaultTableStyleNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf die Sammlung der Tabellestile zu
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            
            // Anzeige des Standard-Tabellenstilnamens
            Console.WriteLine("Default Table Style: " + tableStyles.DefaultTableStyleName);
            
            // Ändert den Standard-Tabellenstil
            tableStyles.DefaultTableStyleName = "TableStyleMedium9";
            Console.WriteLine("New Default Table Style: " + tableStyles.DefaultTableStyleName);
            
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


