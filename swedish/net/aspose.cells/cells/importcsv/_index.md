---
title: "Cells.ImportCSV"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Importera en CSV-fil till cellerna"
type: docs
url: /sv/net/aspose.cells/cells/importcsv/
---
## ImportCSV(string, string, bool, int, int) {#importcsv_3}

Importera en CSV-fil till cellerna.

```csharp
public void ImportCSV(string fileName, string splitter, bool convertNumericData, int firstRow, 
    int firstColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | CSV-filnamnet. |
| delare | String | Delaren |
| convertNumericData | Boolean | Om strängen i textfilen konverteras till numerisk data. |
| firstRow | Int32 | Radnumret för den första cellen att importera i. |
| firstColumn | Int32 | Kolumnnumret för den första cellen att importera i. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportCSVWithStringStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Sökväg till CSV-filen
            string csvPath = "example.csv";
            
            // Importera CSV-data med start i cell A1 (rad 0, kolumn 0)
            // Använder semikolon som avgränsare och konverterar numerisk data
            cells.ImportCSV(csvPath, ";", true, 0, 0);

            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCSV(Stream, string, bool, int, int) {#importcsv_1}

Importera en CSV-fil till cellerna.

```csharp
public void ImportCSV(Stream stream, string splitter, bool convertNumericData, int firstRow, 
    int firstColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | CSV-filströmmen. |
| delare | String | Delaren |
| convertNumericData | Boolean | Om strängen i textfilen konverteras till numerisk data. |
| firstRow | Int32 | Radnumret för den första cellen att importera i. |
| firstColumn | Int32 | Kolumnnumret för den första cellen att importera i. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsMethodImportCSVWithStreamStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa exempel-CSV-data i minnet
            string csvData = "Name,Age,City\nJohn,30,New York\nAlice,25,London\nBob,35,Paris";
            byte[] byteArray = System.Text.Encoding.UTF8.GetBytes(csvData);
            MemoryStream csvStream = new MemoryStream(byteArray);

            try
            {
                // Anropa ImportCSV-metoden med parametrarna Stream, String, Boolean, Int32, Int32
                cells.ImportCSV(csvStream, ",", true, 0, 0);

                Console.WriteLine("CSV data imported successfully to worksheet.");
                Console.WriteLine($"Data range: A1 to {cells.MaxDisplayRange}");

                // Spara arbetsboken
                workbook.Save("ImportCSVFromStreamDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing CSV: {ex.Message}");
            }
            finally
            {
                csvStream?.Dispose();
            }
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCSV(string, TxtLoadOptions, int, int) {#importcsv_2}

Importera en CSV-fil till cellerna.

```csharp
public void ImportCSV(string fileName, TxtLoadOptions options, int firstRow, int firstColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | String | CSV-filnamnet. |
| alternativ | TxtLoadOptions | Läsalternativen för att läsa textfilen |
| firstRow | Int32 | Radnumret för den första cellen att importera i. |
| firstColumn | Int32 | Kolumnnumret för den första cellen att importera i. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportCSVWithStringTxtLoadOptionsInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa CSV-läsalternativ
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.Separator = ',';
            loadOptions.ConvertDateTimeData = true;
            loadOptions.ConvertNumericData = true;
            loadOptions.ParsingFormulaOnOpen = true;

            // Exempel på CSV-filsökväg (ersätt med den faktiska sökvägen i din miljö)
            string csvFilePath = "example.csv";
            
            // Importera CSV-data med start i cell A1 (rad 0, kolumn 0)
            worksheet.Cells.ImportCSV(csvFilePath, loadOptions, 0, 0);

            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCSV(Stream, TxtLoadOptions, int, int) {#importcsv}

Importera en CSV-fil till cellerna.

```csharp
public void ImportCSV(Stream stream, TxtLoadOptions options, int firstRow, int firstColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | CSV-filströmmen. |
| alternativ | TxtLoadOptions | Läsalternativen för att läsa textfilen |
| firstRow | Int32 | Radnumret för den första cellen att importera i. |
| firstColumn | Int32 | Kolumnnumret för den första cellen att importera i. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsMethodImportCSVWithStreamTxtLoadOptionsInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta Cells-samlingen
            Cells cells = worksheet.Cells;

            // Skapa exempel-CSV-data
            string csvData = "Name,Age,City\nJohn,30,New York\nJane,25,Los Angeles\nBob,35,Chicago";

            // Skapa en minnesström med CSV-data
            MemoryStream csvStream = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData));

            try
            {
                // Skapa TxtLoadOptions för CSV-import
                TxtLoadOptions loadOptions = new TxtLoadOptions();
                loadOptions.Separator = ',';
                loadOptions.ConvertNumericData = true;

                // Importera CSV-data med start i rad 0, kolumn 0
                cells.ImportCSV(csvStream, loadOptions, 0, 0);

                // Spara arbetsboken
                workbook.Save("ImportCSVDemo.xlsx");

                Console.WriteLine("CSV data imported successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing CSV: {ex.Message}");
            }
            finally
            {
                // Avsluta strömmen
                csvStream.Dispose();
            }
        }
    }
}
```

### Se även

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


