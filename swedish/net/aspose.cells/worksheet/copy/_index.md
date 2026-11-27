---
title: "Worksheet.Copy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Kopierar innehåll och format från ett annat arbetsblad"
type: docs
url: /sv/net/aspose.cells/worksheet/copy/
---
## Copy(Worksheet) {#copy}

Kopierar innehåll och format från ett annat kalkylblad.

```csharp
public void Copy(Worksheet sourceSheet)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceSheet | Arbetsblad | Källarbetsblad. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCopyWithWorksheetDemo
    {
        public static void Run()
        {
            // Skapa en källarbetsbok med exempeldata
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Worksheet");
            
            // Skapa en målarbetsbok
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Kopiera källarbetsbladet till destinationsarbetsbladet
            destSheet.Copy(sourceSheet);
            
            // Spara resultatet
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Worksheet, CopyOptions) {#copy_1}

Kopierar innehåll och format från ett annat kalkylblad.

```csharp
public void Copy(Worksheet sourceSheet, CopyOptions copyOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceSheet | Arbetsblad | Källarbetsblad. |
| copyOptions | CopyOptions |  |

### Anmärkningar

Du kan kopiera data från ett annat arbetsblad i samma fil eller en annan fil. Denna metod stöder dock inte att kopiera ritobjekt, såsom kommentarer, bilder och diagram.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCopyWithWorksheetCopyOptionsDemo
    {
        public static void Run()
        {
            // Skapa källarbetsbok med exempeldata
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Name = "SourceSheet";
            srcSheet.Cells["A1"].PutValue("Source Data");

            // Skapa målarbetsbok
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            destSheet.Name = "DestinationSheet";

            // Konfigurera kopieringsalternativ
            CopyOptions options = new CopyOptions();
            options.ReferToDestinationSheet = true;

            // Kopiera arbetsblad med alternativ
            srcSheet.Copy(destSheet, options);

            // Verifiera kopieringsoperationen
            Console.WriteLine("Copied cell value: " + destSheet.Cells["A1"].StringValue);
            
            // Spara resultatet
            destWorkbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [CopyOptions](../../copyoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


