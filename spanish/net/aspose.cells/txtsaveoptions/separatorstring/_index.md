---
title: "TxtSaveOptions.SeparatorString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtSaveOptions. Obtiene y establece un valor de cadena como separador"
type: docs
url: /es/net/aspose.cells/txtsaveoptions/separatorstring/
---
## TxtSaveOptions.SeparatorString property

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
    public class TxtSaveOptionsPropertySeparatorStringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de muestra con datos de prueba
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de prueba
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["A3"].PutValue(1);
            worksheet.Cells["B3"].PutValue(2);

            // Guardar con separador de espacio
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.SeparatorString = " ";
            workbook.Save("output_space.txt", saveOptions);

            // Guardar con separador de barra vertical
            saveOptions.SeparatorString = "|";
            workbook.Save("output_pipe.txt", saveOptions);

            // Cargar el archivo separado por espacios para verificar
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.SeparatorString = " ";
            Workbook loadedWorkbook = new Workbook("output_space.txt", loadOptions);
            Cells cells = loadedWorkbook.Worksheets[0].Cells;

            Console.WriteLine("Space-separated values:");
            Console.WriteLine($"{cells["A1"].StringValue} {cells["B1"].StringValue}");
            Console.WriteLine($"{cells["A2"].StringValue} {cells["B2"].StringValue}");
            Console.WriteLine($"{cells["A3"].IntValue} {cells["B3"].IntValue}");
        }
    }
}
```

### Ver también

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


