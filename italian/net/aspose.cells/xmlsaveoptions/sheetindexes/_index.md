---
title: "XmlSaveOptions.SheetIndexes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XmlSaveOptions. Rappresenta gli indici dei fogli esportati"
type: docs
url: /it/net/aspose.cells/xmlsaveoptions/sheetindexes/
---
## XmlSaveOptions.SheetIndexes property

Rappresenta gli indici dei fogli esportati.

```csharp
public int[] SheetIndexes { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con più fogli
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Popola alcuni dati in tutti i fogli
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue("Data in " + sheet.Name);
            }

            // Crea un'istanza di XmlSaveOptions
            XmlSaveOptions options = new XmlSaveOptions();

            // Inizialmente esporta tutti i fogli (SheetIndexes è null)
            Console.WriteLine("Initial SheetIndexes value: " + (options.SheetIndexes == null ? "null (all sheets)" : string.Join(",", options.SheetIndexes)));

            // Imposta per esportare solo il primo e il terzo foglio (indici 0 e 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // Salva solo i fogli selezionati
            workbook.Save("XmlExportSelectedSheets.xml", options);

            // Modifica per esportare solo il secondo foglio (indice 1)
            options.SheetIndexes = new int[] { 1 };

            // Salva con una selezione di fogli diversa
            workbook.Save("XmlExportSingleSheet.xml", options);

            // Imposta SheetIndexes a null per esportare tutti i fogli
            options.SheetIndexes = null;
            workbook.Save("XmlExportAllSheets.xml", options);
        }
    }
}
```

### Vedi anche

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


