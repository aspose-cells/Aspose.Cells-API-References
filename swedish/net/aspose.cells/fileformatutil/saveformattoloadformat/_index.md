---
title: "FileFormatUtil.SaveFormatToLoadFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FileFormatUtil‑metod. Konverterar ett SaveFormat‑värde till ett LoadFormat‑värde om möjligt"
type: docs
url: /sv/net/aspose.cells/fileformatutil/saveformattoloadformat/
---
## FileFormatUtil.SaveFormatToLoadFormat method

Konverterar ett SaveFormat‑värde till ett LoadFormat‑värde om möjligt.

```csharp
public static LoadFormat SaveFormatToLoadFormat(SaveFormat saveFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveFormat | SaveFormat | Sparaformatet. |

### Returvärde

Läsformatet

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodSaveFormatToLoadFormatWithSaveFormatDemo
    {
        public static void Run()
        {
            // Demonstrera SaveFormatToLoadFormat‑konverteringar
            Console.WriteLine("SaveFormat to LoadFormat Conversion Examples:");
            
            LoadFormat excel97To2003 = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Excel97To2003);
            Console.WriteLine($"SaveFormat.Excel97To2003 -> {excel97To2003}");

            LoadFormat xlsx = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Xlsx);
            Console.WriteLine($"SaveFormat.Xlsx -> {xlsx}");

            LoadFormat tsv = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Tsv);
            Console.WriteLine($"SaveFormat.Tsv -> {tsv}");

            LoadFormat ods = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Ods);
            Console.WriteLine($"SaveFormat.Ods -> {ods}");

            LoadFormat xlsb = FileFormatUtil.SaveFormatToLoadFormat(SaveFormat.Xlsb);
            Console.WriteLine($"SaveFormat.Xlsb -> {xlsb}");
        }
    }
}
```

### Se även

* enum [LoadFormat](../../loadformat/)
* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


