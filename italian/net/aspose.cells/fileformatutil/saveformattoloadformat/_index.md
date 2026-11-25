---
title: "FileFormatUtil.SaveFormatToLoadFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FileFormatUtil. Converte un valore SaveFormat in un valore LoadFormat, se possibile"
type: docs
url: /it/net/aspose.cells/fileformatutil/saveformattoloadformat/
---
## FileFormatUtil.SaveFormatToLoadFormat method

Converte un valore SaveFormat in un valore LoadFormat, se possibile.

```csharp
public static LoadFormat SaveFormatToLoadFormat(SaveFormat saveFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveFormat | SaveFormat | Il formato di salvataggio. |

### Valore di ritorno

Il formato di caricamento

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodSaveFormatToLoadFormatWithSaveFormatDemo
    {
        public static void Run()
        {
            // Dimostra le conversioni SaveFormatToLoadFormat
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

### Vedi anche

* enum [LoadFormat](../../loadformat/)
* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


