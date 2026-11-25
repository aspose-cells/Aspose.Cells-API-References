---
title: "TxtSaveOptions.KeepSeparatorsForBlankRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtSaveOptions. Indica se i separatori devono essere emessi per una riga vuota. Il valore predefinito è false, quindi per impostazione predefinita il contenuto della riga vuota sarà vuoto"
type: docs
url: /it/net/aspose.cells/txtsaveoptions/keepseparatorsforblankrow/
---
## TxtSaveOptions.KeepSeparatorsForBlankRow property

Indica se i separatori devono essere emessi per una riga vuota. Il valore predefinito è false, quindi per impostazione predefinita il contenuto della riga vuota sarà vuoto.

```csharp
public bool KeepSeparatorsForBlankRow { get; set; }
```

### Esempi

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyKeepSeparatorsForBlankRowDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Aggiungi alcuni dati con righe vuote
            cells[0, 0].PutValue("a");
            cells[0, 1].PutValue("b");
            cells[3, 0].PutValue("c");
            cells[4, 1].PutValue("d");

            // Crea le opzioni di salvataggio con KeepSeparatorsForBlankRow impostato a true
            TxtSaveOptions options = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                KeepSeparatorsForBlankRow = true
            };

            // Salva la cartella di lavoro in CSV con le opzioni
            string csvOutput = SaveAsCsv(wb, options);
            Console.WriteLine(csvOutput);
        }

        private static string SaveAsCsv(Workbook wb, TxtSaveOptions options)
        {
            using (System.IO.MemoryStream stream = new System.IO.MemoryStream())
            {
                wb.Save(stream, options);
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


