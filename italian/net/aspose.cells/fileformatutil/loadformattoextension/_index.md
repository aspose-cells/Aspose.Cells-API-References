---
title: "FileFormatUtil.LoadFormatToExtension"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FileFormatUtil. Converte un valore enumerato di formato di caricamento in un'estensione di file"
type: docs
url: /it/net/aspose.cells/fileformatutil/loadformattoextension/
---
## FileFormatUtil.LoadFormatToExtension method

Converte un valore enumerato di LoadFormat in un'estensione di file.

```csharp
public static string LoadFormatToExtension(LoadFormat loadFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadFormat | LoadFormat | Il formato del file caricato. |

### Valore di ritorno

L'estensione restituita è una stringa in minuscolo con un punto iniziale.

### Osservazioni

Se non può essere convertito, restituisce null.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodLoadFormatToExtensionWithLoadFormatDemo
    {
        public static void Run()
        {
            // Dimostra LoadFormatToExtension con vari valori di LoadFormat
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

### Vedi anche

* enum [LoadFormat](../../loadformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


