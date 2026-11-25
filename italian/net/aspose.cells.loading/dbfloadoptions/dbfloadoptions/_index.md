---
title: "DbfLoadOptions.DbfLoadOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore DbfLoadOptions. Le opzioni"
type: docs
url: /it/net/aspose.cells.loading/dbfloadoptions/dbfloadoptions/
---
## DbfLoadOptions constructor

Le opzioni.

```csharp
public DbfLoadOptions()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;
    using System;

    public class DbfLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un'istanza di DbfLoadOptions usando il metodo #ctor
                DbfLoadOptions loadOptions = new DbfLoadOptions();

                // Crea una cartella di lavoro con le opzioni di caricamento DBF
                Workbook workbook = new Workbook("sample.dbf", loadOptions);

                // Accedi al primo foglio di lavoro
                Worksheet worksheet = workbook.Worksheets[0];

                // Visualizza alcuni dati dal file DBF caricato
                Console.WriteLine("Data loaded from DBF file:");
                Console.WriteLine(worksheet.Cells["A1"].StringValue);

                // Salva la cartella di lavoro in formato Excel
                workbook.Save("DbfLoadOptionsCtorDemo.xlsx", SaveFormat.Xlsx);
                Console.WriteLine("File saved successfully with DBF data");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DbfLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [DbfLoadOptions](../)
* namespace [Aspose.Cells.Loading](../../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../../)


