---
title: "Cells.CopyRows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Kopierar data och format för några hela rader"
type: docs
url: /sv/net/aspose.cells/cells/copyrows/
---
## CopyRows(Cells, int, int, int) {#copyrows}

Kopierar data och format för några hela rader.

```csharp
public void CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceCells | Celler | Source Cells-objektet innehåller data och format att kopiera. |
| sourceRowIndex | Int32 | Källradens index. |
| destinationRowIndex | Int32 | Målradsindex. |
| rowNumber | Int32 | Det kopierade radnumret. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowsWithCellsInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook destinationWorkbook = new Workbook();
            Workbook sourceWorkbook = new Workbook();

            // Lägg till exempeldata i källarboken
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data 1");
            sourceSheet.Cells["A2"].PutValue("Source Data 2");
            sourceSheet.Cells["A3"].PutValue("Source Data 3");

            // Hämta cellerna från båda arbetsböckerna
            Cells destinationCells = destinationWorkbook.Worksheets[0].Cells;
            Cells sourceCells = sourceSheet.Cells;

            // Kopiera alla rader från källan till destinationen med start i rad 0 i destinationen
            destinationCells.CopyRows(sourceCells, 0, 0, sourceCells.MaxDisplayRange.RowCount);

            // Spara resultatet
            destinationWorkbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions) {#copyrows_1}

Kopierar data och format för några hela rader.

```csharp
public void CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, 
    CopyOptions copyOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceCells | Celler | Source Cells-objektet innehåller data och format att kopiera. |
| sourceRowIndex | Int32 | Källradens index. |
| destinationRowIndex | Int32 | Målradsindex. |
| rowNumber | Int32 | Det kopierade radnumret. |
| copyOptions | CopyOptions | Kopieringsalternativen. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowsWithCellsInt32Int32Int32CopyOptionDemo2
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata och hyperlänkar
            worksheet.Cells["A1"].PutValue("Source Data");
            worksheet.Cells["A4"].PutValue("Row 4 Data");
            worksheet.Hyperlinks.Add("A4", 1, 1, "https://www.example.com");

            // Infoga en tom rad på rad 5
            worksheet.Cells.InsertRows(5, 1);

            // Kopiera rad 4 till rad 5 utan CopyOptions
            worksheet.Cells.CopyRows(worksheet.Cells, 4, 5, 1);
            Console.WriteLine("Hyperlinks count after copy without options: " + worksheet.Hyperlinks.Count);

            // Återställ kalkylbladet
            worksheet.Cells.ClearContents(0, 0, worksheet.Cells.MaxRow + 1, worksheet.Cells.MaxColumn + 1);
            worksheet.Hyperlinks.Clear();
            worksheet.Cells["A4"].PutValue("Row 4 Data");
            worksheet.Hyperlinks.Add("A4", 1, 1, "https://www.example.com");

            // Infoga en tom rad på rad 5 igen
            worksheet.Cells.InsertRows(5, 1);

            // Kopiera rad 4 till rad 5 med CopyOptions
            CopyOptions options = new CopyOptions();
            options.ExtendToAdjacentRange = true;
            worksheet.Cells.CopyRows(worksheet.Cells, 4, 5, 1, options);
            Console.WriteLine("Hyperlinks count after copy with options: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### Se även

* class [CopyOptions](../../copyoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions, PasteOptions) {#copyrows_2}

Kopierar data och format för några hela rader.

```csharp
public void CopyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, 
    int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceCells0 | Celler | Source Cells-objektet innehåller data och format att kopiera. |
| sourceRowIndex | Int32 | Källradens index. |
| destinationRowIndex | Int32 | Målradsindex. |
| rowNumber | Int32 | Det kopierade radnumret. |
| copyOptions | CopyOptions | Kopieringsalternativen. |
| pasteOptions | PasteOptions | alternativen för inklistring. |

### Se även

* class [CopyOptions](../../copyoptions/)
* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


