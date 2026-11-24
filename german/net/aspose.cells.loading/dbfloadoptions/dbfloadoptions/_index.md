---
title: "DbfLoadOptions.DbfLoadOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DbfLoadOptions‑Konstruktor. Die Optionen"
type: docs
url: /de/net/aspose.cells.loading/dbfloadoptions/dbfloadoptions/
---
## DbfLoadOptions constructor

Die Optionen.

```csharp
public DbfLoadOptions()
```

### Beispiele

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
                // Erstelle eine DbfLoadOptions‑Instanz mit der #ctor‑Methode
                DbfLoadOptions loadOptions = new DbfLoadOptions();

                // Arbeitsmappe mit DBF-Ladeoptionen erstellen
                Workbook workbook = new Workbook("sample.dbf", loadOptions);

                // Greife auf das erste Arbeitsblatt zu
                Worksheet worksheet = workbook.Worksheets[0];

                // Zeige einige Daten aus der geladenen DBF‑Datei an
                Console.WriteLine("Data loaded from DBF file:");
                Console.WriteLine(worksheet.Cells["A1"].StringValue);

                // Arbeitsmappe im Excel-Format speichern
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

### Siehe auch

* class [DbfLoadOptions](../)
* namespace [Aspose.Cells.Loading](../../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../../)


