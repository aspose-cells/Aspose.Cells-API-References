---
title: "FileFormatUtil.IsTemplateFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FileFormatUtil. Devuelve true si la extensión es .xlt .xltX .xltm.ots"
type: docs
url: /es/net/aspose.cells/fileformatutil/istemplateformat/
---
## FileFormatUtil.IsTemplateFormat method

Devuelve true si la extensión es .xlt, .xltX, .xltm, .ots.

```csharp
public static bool IsTemplateFormat(string extension)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| extensión | String |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFormatUtilMethodIsTemplateFormatWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            string extension = ".xltx";

            try
            {
                bool isTemplate = FileFormatUtil.IsTemplateFormat(extension);
                Console.WriteLine($"Is '{extension}' a template format? {isTemplate}");

                if (isTemplate)
                {
                    SaveFormat saveFormat = FileFormatUtil.ExtensionToSaveFormat(extension);
                    workbook.Save($"IsTemplateFormatDemo{extension}", saveFormat);
                    Console.WriteLine($"Workbook saved as template format: {extension}");
                }
            }
            catch (ArgumentException argEx)
            {
                Console.WriteLine($"Invalid argument: {argEx.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


