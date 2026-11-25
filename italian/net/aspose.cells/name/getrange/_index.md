---
title: "Name.GetRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Name. Ottiene l'intervallo se questo nome fa riferimento a un intervallo"
type: docs
url: /it/net/aspose.cells/name/getrange/
---
## GetRange() {#getrange}

Ottiene l'intervallo se questo nome si riferisce a un intervallo.

```csharp
public Range GetRange()
```

### Valore di ritorno

L'intervallo.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            
            // Crea un intervallo denominato
            int index = workbook.Worksheets.Names.Add("MyRange");
            workbook.Worksheets.Names[index].RefersTo = "=Sheet1!A1:B3";
            Name namedRange = workbook.Worksheets.Names[index];
            
            // Dimostra il metodo GetRange
            Aspose.Cells.Range range = namedRange.GetRange();
            Console.WriteLine("Named Range Address: " + range.Address);
            Console.WriteLine("Worksheet Name: " + range.Worksheet.Name);
            
            // Modifica l'intervallo
            foreach (Cell cell in range)
            {
                if (cell.Row == 0)
                {
                    cell.PutValue(cell.StringValue.ToUpper());
                }
            }
            
            // Salva la cartella di lavoro
            workbook.Save("NamedRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRange(bool) {#getrange_1}

Ottiene l'intervallo se questo nome si riferisce a un intervallo

```csharp
public Range GetRange(bool recalculate)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ricalcola | Booleano | se ricalcolarlo se questo nome è stato calcolato prima di questa invocazione. |

### Valore di ritorno

L'intervallo.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeWithBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Popola dati di esempio
            for (int i = 0; i < 4; i++)
            {
                cells[i, 1].PutValue(i); // Column B values: 0,1,2,3
            }

            // Crea un intervallo denominato con formula
            int nameIndex = wb.Worksheets.Names.Add("testname");
            Name name = wb.Worksheets.Names[nameIndex];
            name.RefersTo = "IFERROR(Sheet1!$B$2:$B$4,-1)";

            // Utilizza l'intervallo denominato nelle formule
            cells["C1"].Formula = "=testname";
            cells["D1"].Formula = "SUM(testname)";

            // Calcola le formule
            wb.CalculateFormula();

            // Ottieni l'intervallo usando GetRange(true)
            Aspose.Cells.Range namedRange = name.GetRange(true);
            Console.WriteLine($"Named range: FirstRow={namedRange.FirstRow}, FirstColumn={namedRange.FirstColumn}, " +
                $"RowCount={namedRange.RowCount}, ColumnCount={namedRange.ColumnCount}");

            // Crea un grafico utilizzando l'intervallo denominato
            int chartIndex = sheet.Charts.Add(ChartType.Column, 10, 1, 20, 5);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("testname", true);
            Console.WriteLine($"Chart data points count: {chart.NSeries[0].CountOfDataValues}");
        }
    }
}
```

### Vedi anche

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRange(int, int, int) {#getrange_2}

Ottiene l'intervallo se questo nome si riferisce a un intervallo. Se il riferimento di questo nome non è assoluto, l'intervallo può variare per celle diverse.

```csharp
public Range GetRange(int sheetIndex, int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | Int32 | L'indice del foglio corrispondente. |
| riga | Int32 | L'indice della riga corrispondente. |
| colonna | Int32 | L'indice della colonna corrispondente |

### Valore di ritorno

L'intervallo.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Dairy");
            
            // Crea un intervallo denominato usando la firma del metodo corretta
            int index = workbook.Worksheets.Names.Add("SubCat");
            workbook.Worksheets.Names["SubCat"].RefersTo = "=" + worksheet.Name + "!A2:A4";
            
            // Ottieni l'intervallo usando GetRange con i parametri riga, colonna e conteggio righe
            Aspose.Cells.Range range = workbook.Worksheets.Names["SubCat"].GetRange(0, 0, 3);
            
            // Visualizza il riferimento dell'intervallo
            Console.WriteLine("Range refers to: " + range.RefersTo);
        }
    }
}
```

### Vedi anche

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


