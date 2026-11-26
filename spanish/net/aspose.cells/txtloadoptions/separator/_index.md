---
title: "TxtLoadOptions.Separator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtLoadOptions. Obtiene y establece el separador de caracteres del archivo de texto"
type: docs
url: /es/net/aspose.cells/txtloadoptions/separator/
---
## TxtLoadOptions.Separator property

Obtiene y establece el separador de caracteres del archivo de texto.

```csharp
public char Separator { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertySeparatorDemo
    {
        public static void Run()
        {
            // Crea datos de ejemplo y guárdalos con un separador personalizado
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.Separator = '*';
            workbook.Save("output.csv", saveOptions);

            // Carga el archivo guardado con el mismo separador
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.Separator = '*';
            Workbook loadedWorkbook = new Workbook("output.csv", loadOptions);

            // Verifica los datos cargados
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];
            Console.WriteLine("A1: " + loadedSheet.Cells["A1"].StringValue);
            Console.WriteLine("B1: " + loadedSheet.Cells["B1"].StringValue);
        }
    }
}
```

### Ver también

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


