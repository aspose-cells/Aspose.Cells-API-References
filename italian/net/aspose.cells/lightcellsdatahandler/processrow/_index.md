---
title: "LightCellsDataHandler.ProcessRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo LightCellsDataHandler. Inizia a elaborare una riga"
type: docs
url: /it/net/aspose.cells/lightcellsdatahandler/processrow/
---
## LightCellsDataHandler.ProcessRow method

Inizia a elaborare una riga.

```csharp
public bool ProcessRow(Row row)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Row | Oggetto riga attualmente in elaborazione. |

### Valore di ritorno

indica se le celle di questa riga devono essere elaborate. false per ignorare tutte le celle in questa riga.

### Osservazioni

Verrà chiamato dopo che le proprietà della riga, come altezza, stile, ...ecc., sono state lette. Tuttavia, le celle di questa riga non sono ancora state lette.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerMethodProcessRowWithRowDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un nuovo workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Aggiungi dati di esempio
                worksheet.Cells["A1"].Value = "Test Data";
                worksheet.Cells["A2"].Value = 100;
                worksheet.Cells["B2"].Value = 200;

                // Crea gestore personalizzato
                var handler = new CustomRowHandler();

                // Elabora la prima riga
                Row firstRow = worksheet.Cells.Rows[0];
                bool result = handler.ProcessRow(firstRow);

                Console.WriteLine($"ProcessRow returned: {result}");
                Console.WriteLine($"Row height after processing: {firstRow.Height}");

                workbook.Save("ProcessRowDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ProcessRow demo: {ex.Message}");
            }
        }

        private class CustomRowHandler : LightCellsDataHandler
        {
            public bool ProcessRow(Row row)
            {
                // Dimostra l'accesso alle proprietà della riga
                Console.WriteLine($"Processing row index: {row.Index}");
                Console.WriteLine($"Row is hidden: {row.IsHidden}");
                Console.WriteLine($"Row is blank: {row.IsBlank}");

                // Modifica l'altezza della riga se non è la riga di intestazione
                if (row.Index > 0)
                {
                    row.Height = 25.0;
                }

                return true;
            }

            public bool StartSheet(Worksheet sheet) => true;
            public bool StartRow(int rowIndex) => true;
            public bool StartCell(int columnIndex) => true;
            public bool ProcessCell(Cell cell) => true;
        }
    }
}
```

### Vedi anche

* class [Row](../../row/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


