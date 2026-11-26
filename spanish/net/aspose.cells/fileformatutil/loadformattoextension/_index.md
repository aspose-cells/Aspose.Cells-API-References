---
title: "FileFormatUtil.LoadFormatToExtension"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FileFormatUtil. Convierte un valor enumerado de formato de carga en una extensión de archivo"
type: docs
url: /es/net/aspose.cells/fileformatutil/loadformattoextension/
---
## FileFormatUtil.LoadFormatToExtension method

Convierte un valor enumerado de formato de carga en una extensión de archivo.

```csharp
public static string LoadFormatToExtension(LoadFormat loadFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loadFormat | LoadFormat | El formato de archivo cargado. |

### Valor de retorno

La extensión devuelta es una cadena en minúsculas con un punto inicial.

### Observaciones

Si no puede ser convertido, devuelve null.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodLoadFormatToExtensionWithLoadFormatDemo
    {
        public static void Run()
        {
            // Demostrar LoadFormatToExtension con varios valores de LoadFormat
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

### Ver también

* enum [LoadFormat](../../loadformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


