---
title: "TableStyleCollection.DefaultTableStyleName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TableStyleCollection. Ottiene e imposta il nome dello stile predefinito della tabella"
type: docs
url: /it/net/aspose.cells.tables/tablestylecollection/defaulttablestylename/
---
## TableStyleCollection.DefaultTableStyleName property

Ottiene e imposta il nome dello stile predefinito della tabella.

```csharp
public string DefaultTableStyleName { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alla raccolta degli stili di tabella
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            
            // Visualizza il nome dello stile di tabella predefinito
            Console.WriteLine("Default Table Style: " + tableStyles.DefaultTableStyleName);
            
            // Modifica lo stile predefinito della tabella
            tableStyles.DefaultTableStyleName = "TableStyleMedium9";
            Console.WriteLine("New Default Table Style: " + tableStyles.DefaultTableStyleName);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


