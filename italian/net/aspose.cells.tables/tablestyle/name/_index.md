---
title: "TableStyle.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TableStyle. Ottiene il nome dello stile di tabella"
type: docs
url: /it/net/aspose.cells.tables/tablestyle/name/
---
## TableStyle.Name property

Ottiene il nome dello stile della tabella.

```csharp
public string Name { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStylePropertyNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alla raccolta degli stili di tabella
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            try
            {
                // Ottieni il primo stile di tabella dalla collezione
                TableStyle tableStyle = tableStyles[0];

                // Visualizza il valore della proprietà Name
                Console.WriteLine("Table Style Name: " + tableStyle.Name);

                // Dimostra l'accesso alla proprietà di sola lettura
                string styleName = tableStyle.Name;
                Console.WriteLine("Retrieved style name: " + styleName);

                // Mostra che possiamo usare il nome per fare riferimento allo stile
                Console.WriteLine("This table style can be referenced by name: " + tableStyle.Name);

                // Salva la cartella di lavoro
                workbook.Save("TableStyleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [TableStyle](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


