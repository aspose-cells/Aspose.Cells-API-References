---
title: "ExportTableOptions.PreprocessExportedValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ExportTableOptions. Preprocessa il valore della cella corrente da esportare"
type: docs
url: /it/net/aspose.cells/exporttableoptions/preprocessexportedvalue/
---
## ExportTableOptions.PreprocessExportedValue method

Preelabora il valore della cella corrente da esportare.

```csharp
public virtual bool PreprocessExportedValue(int cellRow, int cellColumn, CellValue value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellRow | Int32 | l'indice di riga della cella corrente |
| cellColumn | Int32 | l'indice di colonna della cella |
| valore | CellValue | valore e tipo della cella corrente |

### Valore di ritorno

Se la cella corrente è stata sostituita con un tipo e/o valore diverso.

### Osservazioni

L'indice di riga e colonna è l'indice assoluto della cella nel foglio di lavoro, non l'indice nella tabella esportata. L'utente può verificare il valore della cella corrente nell'implementazione di override di questo metodo; se la cella corrente deve essere sostituita con un altro tipo e valore, l'implementazione deve impostare il tipo e il valore attesi sull'oggetto CellValue e restituire true. Per impostazione predefinita questo metodo non fa nulla e restituisce false.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExportTableOptionsMethodPreprocessExportedValueWithInt32Int32CellValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio nel foglio di lavoro
            worksheet.Cells["A1"].PutValue("Test Value");
            worksheet.Cells["A2"].PutValue(123.45);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            // Crea un'istanza di ExportTableOptions
            ExportTableOptions exportOptions = new ExportTableOptions();

            // Crea un oggetto CellValue per dimostrazione
            CellValue cellValue = new CellValue();
            cellValue.Type = CellValueType.IsString;
            cellValue.Value = "Processed Value";

            try
            {
                // Chiama PreprocessExportedValue con parametri specifici (riga 0, colonna 0, CellValue)
                bool result = exportOptions.PreprocessExportedValue(0, 0, cellValue);

                // Visualizza il risultato della chiamata al metodo
                Console.WriteLine($"PreprocessExportedValue returned: {result}");

                // Modifica la cella con il valore elaborato se necessario
                if (result)
                {
                    worksheet.Cells[0, 0].PutValue(cellValue.Value);
                }

                // Salva la cartella di lavoro
                workbook.Save("PreprocessExportedValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PreprocessExportedValue method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [CellValue](../../cellvalue/)
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


