---
title: "DbfLoadOptions.DbfLoadOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de DbfLoadOptions. Las opciones"
type: docs
url: /es/net/aspose.cells.loading/dbfloadoptions/dbfloadoptions/
---
## DbfLoadOptions constructor

Las opciones.

```csharp
public DbfLoadOptions()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;
    using System;

    public class DbfLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            try
            {
                // Cree una instancia de DbfLoadOptions usando el método #ctor
                DbfLoadOptions loadOptions = new DbfLoadOptions();

                // Crear libro de trabajo con opciones de carga DBF
                Workbook workbook = new Workbook("sample.dbf", loadOptions);

                // Acceder a la primera hoja de cálculo
                Worksheet worksheet = workbook.Worksheets[0];

                // Muestre algunos datos del archivo DBF cargado
                Console.WriteLine("Data loaded from DBF file:");
                Console.WriteLine(worksheet.Cells["A1"].StringValue);

                // Guardar el libro de trabajo en formato Excel
                workbook.Save("DbfLoadOptionsCtorDemo.xlsx", SaveFormat.Xlsx);
                Console.WriteLine("File saved successfully with DBF data");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DbfLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [DbfLoadOptions](../)
* namespace [Aspose.Cells.Loading](../../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../../)


