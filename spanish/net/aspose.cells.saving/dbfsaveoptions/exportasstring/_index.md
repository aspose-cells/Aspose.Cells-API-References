---
title: "DbfSaveOptions.ExportAsString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "DbfSaveOptions property. Indica si se exporta como valor de cadena"
type: docs
url: /es/net/aspose.cells.saving/dbfsaveoptions/exportasstring/
---
## DbfSaveOptions.ExportAsString property

Indica si se exporta como valor de cadena

```csharp
public bool ExportAsString { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class DbfSaveOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra con tipos mixtos
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("TextValue");

            // Crear instancia de DbfSaveOptions
            DbfSaveOptions options = new DbfSaveOptions();

            // Mostrar valor actual de ExportAsString
            Console.WriteLine("Current ExportAsString value: " + options.ExportAsString);

            // Establecer ExportAsString a true (todos los valores se exportarán como cadenas)
            options.ExportAsString = true;
            Console.WriteLine("ExportAsString set to: " + options.ExportAsString);

            // Guardar con ExportAsString = true
            workbook.Save("ExportAsStringTrue.dbf", options);

            // Establecer ExportAsString a false (los valores mantendrán sus tipos originales)
            options.ExportAsString = false;
            Console.WriteLine("ExportAsString set to: " + options.ExportAsString);

            // Guardar con ExportAsString = false
            workbook.Save("ExportAsStringFalse.dbf", options);
        }
    }
}
```

### Ver también

* class [DbfSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


