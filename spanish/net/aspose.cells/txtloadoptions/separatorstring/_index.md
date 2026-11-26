---
title: "TxtLoadOptions.SeparatorString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtLoadOptions. Obtiene y establece un valor de cadena como separador"
type: docs
url: /es/net/aspose.cells/txtloadoptions/separatorstring/
---
## TxtLoadOptions.SeparatorString property

Obtiene y establece un valor de cadena como separador.

```csharp
public string SeparatorString { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertySeparatorStringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establece datos de ejemplo con separador personalizado
            worksheet.Cells["A1"].PutValue("John&Doe");
            worksheet.Cells["B1"].PutValue("30");
            worksheet.Cells["A2"].PutValue("Jane&Smith");
            worksheet.Cells["B2"].PutValue("25");

            // Guarda con separador personalizado
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.SeparatorString = "&";
            workbook.Save("output.csv", saveOptions);

            // Carga con el mismo separador
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.SeparatorString = "&";
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


