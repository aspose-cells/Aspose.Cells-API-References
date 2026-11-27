---
title: "FileFormatUtil.LoadFormatToExtension"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FileFormatUtil‑metod. Konverterar ett laddningsformat‑enumerationsvärde till en filändelse"
type: docs
url: /sv/net/aspose.cells/fileformatutil/loadformattoextension/
---
## FileFormatUtil.LoadFormatToExtension method

Konverterar ett LoadFormat‑enumererat värde till en filändelse.

```csharp
public static string LoadFormatToExtension(LoadFormat loadFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadFormat | LoadFormat | Det laddade filformatet. |

### Returvärde

Den returnerade filändelsen är en gemenerad sträng med en inledande punkt.

### Anmärkningar

Om det inte kan konverteras returneras null.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodLoadFormatToExtensionWithLoadFormatDemo
    {
        public static void Run()
        {
            // Demonstrera LoadFormatToExtension med olika LoadFormat‑värden
            Console.WriteLine("Auto format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Auto));
            Console.WriteLine("CSV format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Csv));
            Console.WriteLine("Excel97-2003 format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Excel97To2003));
            Console.WriteLine("XLSX format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Xlsx));
            Console.WriteLine("TSV format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Tsv));
            Console.WriteLine("ODS format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Ods));
            Console.WriteLine("XLSB format extension: " + FileFormatUtil.LoadFormatToExtension(LoadFormat.Xlsb));
        }
    }
}
```

### Se även

* enum [LoadFormat](../../loadformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


