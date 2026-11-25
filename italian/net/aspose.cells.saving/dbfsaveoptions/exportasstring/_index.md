---
title: "DbfSaveOptions.ExportAsString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DbfSaveOptions. Indica se esportare come valore stringa"
type: docs
url: /it/net/aspose.cells.saving/dbfsaveoptions/exportasstring/
---
## DbfSaveOptions.ExportAsString property

Indica se esportare come valore stringa

```csharp
public bool ExportAsString { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class DbfSaveOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio con tipi misti
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("TextValue");

            // Crea un'istanza di DbfSaveOptions
            DbfSaveOptions options = new DbfSaveOptions();

            // Mostra il valore corrente di ExportAsString
            Console.WriteLine("Current ExportAsString value: " + options.ExportAsString);

            // Imposta ExportAsString su true (tutti i valori saranno esportati come stringhe)
            options.ExportAsString = true;
            Console.WriteLine("ExportAsString set to: " + options.ExportAsString);

            // Salva con ExportAsString = true
            workbook.Save("ExportAsStringTrue.dbf", options);

            // Imposta ExportAsString su false (i valori manterranno i loro tipi originali)
            options.ExportAsString = false;
            Console.WriteLine("ExportAsString set to: " + options.ExportAsString);

            // Salva con ExportAsString = false
            workbook.Save("ExportAsStringFalse.dbf", options);
        }
    }
}
```

### Vedi anche

* class [DbfSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


