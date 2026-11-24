---
title: "FileFormatUtil.SaveFormatToLoadFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FileFormatUtil-Methode. Konvertiert einen SaveFormat-Wert in einen LoadFormat-Wert, falls möglich"
type: docs
url: /de/net/aspose.cells/fileformatutil/saveformattoloadformat/
---
## FileFormatUtil.SaveFormatToLoadFormat method

Konvertiert einen SaveFormat-Wert, falls möglich, in einen LoadFormat-Wert.

```csharp
public static LoadFormat SaveFormatToLoadFormat(SaveFormat saveFormat)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| saveFormat | SaveFormat | Das Speicherformat. |

### Rückgabewert

Das Ladeformat.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodSaveFormatToLoadFormatWithSaveFormatDemo
    {
        public static void Run()
        {
            // Demonstriere SaveFormatToLoadFormat-Konvertierungen
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

### Siehe auch

* enum [LoadFormat](../../loadformat/)
* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


