---
title: "FileFormatUtil.SaveFormatToLoadFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FileFormatUtil. Convierte un valor SaveFormat a un valor LoadFormat si es posible"
type: docs
url: /es/net/aspose.cells/fileformatutil/saveformattoloadformat/
---
## FileFormatUtil.SaveFormatToLoadFormat method

Convierte un valor SaveFormat a un valor LoadFormat si es posible.

```csharp
public static LoadFormat SaveFormatToLoadFormat(SaveFormat saveFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveFormat | SaveFormat | El formato de guardado. |

### Valor de retorno

El formato de carga

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodSaveFormatToLoadFormatWithSaveFormatDemo
    {
        public static void Run()
        {
            // Demostrar conversiones SaveFormatToLoadFormat
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

### Ver también

* enum [LoadFormat](../../loadformat/)
* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


