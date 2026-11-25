---
title: "ChartCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ChartCollection. Aggiunge un grafico alla collezione"
type: docs
url: /it/net/aspose.cells.charts/chartcollection/add/
---
## Add(ChartType, int, int, int, int) {#add}

Aggiunge un grafico alla raccolta.

```csharp
public int Add(ChartType type, int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | ChartType | Tipo di grafico |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| bottomRow | Int32 | Indice della riga in basso a destra |
| rightColumn | Int32 | Indice della colonna in basso a destra |

### Valore di ritorno

[`Chart`](../../chart/) object index.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodAddWithChartTypeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 1; i <= 10; i++)
            {
                sheet.Cells["A" + (i + 1)].PutValue("Cat " + i);
                sheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // Aggiungi un grafico usando i parametri specificati
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 2, 25, 11);
            Chart chart = sheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("=Sheet1!$A$1:$B$11", true);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(ChartType, string, int, int, int, int) {#add_2}

Aggiunge un grafico alla raccolta.

```csharp
[Obsolete("Use ChartCollection.Add(ChartType, string, bool ,int , int, int, int ) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(ChartType type, string dataRange, int topRow, int leftColumn, int rightRow, 
    int bottomColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | ChartType | Tipo di grafico |
| dataRange | String | Specifica l'intervallo di dati del grafico |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| rightRow | Int32 | Indice della riga in basso a destra |
| bottomColumn | Int32 | Indice della colonna in basso a destra |

### Valore di ritorno

[`Chart`](../../chart/) object index.

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, utilizza la proprietà `Add`. Questa proprietà sarà rimossa tra 12 mesi a partire da maggio 2022. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionMethodAddWithChartTypeStringInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            try
            {
                // Chiama il metodo Add con i parametri (ChartType, String, Int32, Int32, Int32, Int32)
                int chartIndex = worksheet.Charts.Add(
                    ChartType.Column,          // Chart type
                    "A1:B4",                  // Data range
                    0,                        // Top row position
                    3,                        // Left column position
                    15,                       // Bottom row position
                    8                         // Right column position
                );

                Console.WriteLine("Chart added successfully at index: " + chartIndex);
                
                // Accedi al grafico appena creato
                Chart chart = worksheet.Charts[chartIndex];
                chart.Title.Text = "Sample Column Chart";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("ChartCollectionMethodAddDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(byte[], string, bool, int, int, int, int) {#add_3}

Aggiunge un grafico con modello predefinito.

```csharp
public int Add(byte[] data, string dataRange, bool isVertical, int topRow, int leftColumn, 
    int rightRow, int bottomColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dati | Byte[] | I dati del file modello del grafico (.crtx). |
| dataRange | String | Specifica l'intervallo di dati del grafico |
| isVertical | Booleano | Specifica se tracciare la serie da un intervallo di valori di cella per riga o per colonna. |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| rightRow | Int32 | Indice della riga in basso a destra |
| bottomColumn | Int32 | Indice della colonna in basso a destra |

### Valore di ritorno

[`Chart`](../../chart/) object index.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionMethodAddWithByteArrayStringBooleanInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Crea un array di byte che rappresenta i dati del grafico (esempio semplificato)
            byte[] chartData = new byte[] { 0x01, 0x02, 0x03 };

            try
            {
                // Chiama il metodo Add con parametri specifici
                int chartIndex = worksheet.Charts.Add(
                    chartData,          // Byte[] data
                    "A1:B4",            // String dataRange
                    true,               // Boolean isVertical
                    0,                  // Int32 topRow
                    0,                  // Int32 leftColumn
                    15,                 // Int32 rightRow
                    8                   // Int32 bottomColumn
                );

                Console.WriteLine($"Chart added successfully at index: {chartIndex}");

                // Accedi al grafico aggiunto
                Chart chart = worksheet.Charts[chartIndex];
                chart.Type = ChartType.Column;

                // Salva il risultato
                workbook.Save("ChartCollectionMethodAddDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(ChartType, string, bool, int, int, int, int) {#add_1}

Aggiunge un grafico alla raccolta.

```csharp
public int Add(ChartType type, string dataRange, bool isVertical, int topRow, int leftColumn, 
    int rightRow, int bottomColumn)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | ChartType | Tipo di grafico |
| dataRange | String | Specifica l'intervallo di dati del grafico |
| isVertical | Booleano | Specifica se tracciare la serie da un intervallo di valori di cella per riga o per colonna. |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| rightRow | Int32 | Indice della riga in basso a destra |
| bottomColumn | Int32 | Indice della colonna in basso a destra |

### Valore di ritorno

[`Chart`](../../chart/) object index.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodAddWithChartTypeStringBooleanInt32IntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["C3"].PutValue(40);

            // Aggiungi il grafico con i parametri specificati
            int chartIndex = worksheet.Charts.Add(ChartType.Column, "A1:C3", true, 4, 4, 14, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


