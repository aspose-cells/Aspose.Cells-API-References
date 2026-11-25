---
title: "TxtSaveOptions.TrimTailingBlankCells"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtSaveOptions. Indica se le celle vuote finali in una riga devono essere eliminate. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/txtsaveoptions/trimtailingblankcells/
---
## TxtSaveOptions.TrimTailingBlankCells property

Indica se le celle vuote finali in una riga devono essere eliminate. Il valore predefinito è false.

```csharp
public bool TrimTailingBlankCells { get; set; }
```

### Osservazioni

Durante il salvataggio in modalità LightCells e se [`ExportArea`](../exportarea/) non è stata specificata, questa opzione non ha effetto e una riga verrà estesa fino all'ultima cella fornita dall'implementazione [`LightCellsDataProvider`](../lightcellsdataprovider/)

### Esempi

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyTrimTailingBlankCellsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Aggiungi dati di esempio
            cells[0, 0].PutValue("A");
            cells[0, 1].PutValue("B");
            cells[0, 2].PutValue("C");
            cells[1, 0].PutValue(1);
            cells[1, 2].PutValue(2);
            cells[2, 0].PutValue(3);

            // Salva senza rimuovere le celle vuote finali (predefinito)
            TxtSaveOptions options1 = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                TrimTailingBlankCells = false
            };
            string result1 = SaveAsCsv(workbook, options1);
            Console.WriteLine("Without TrimTailingBlankCells:\n" + result1);

            // Salva rimuovendo le celle vuote finali
            TxtSaveOptions options2 = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                TrimTailingBlankCells = true
            };
            string result2 = SaveAsCsv(workbook, options2);
            Console.WriteLine("\nWith TrimTailingBlankCells:\n" + result2);
        }

        private static string SaveAsCsv(Workbook workbook, TxtSaveOptions options)
        {
            using (System.IO.MemoryStream stream = new System.IO.MemoryStream())
            {
                workbook.Save(stream, options);
                return Encoding.ASCII.GetString(stream.ToArray());
            }
        }
    }
}
```

### Vedi anche

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


