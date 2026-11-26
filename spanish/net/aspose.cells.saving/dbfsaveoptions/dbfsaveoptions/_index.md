---
title: "DbfSaveOptions.DbfSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "DbfSaveOptions constructor. Las opciones de guardado del archivo .dbf"
type: docs
url: /es/net/aspose.cells.saving/dbfsaveoptions/dbfsaveoptions/
---
## DbfSaveOptions constructor

Las opciones de guardado del archivo .dbf.

```csharp
public DbfSaveOptions()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class DbfSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            try
            {
                // Crear una instancia de DbfSaveOptions usando el constructor
                DbfSaveOptions saveOptions = new DbfSaveOptions();
                
                // Establecer propiedades de las opciones de guardado
                saveOptions.ExportAsString = true;
                
                // Guardar el libro de trabajo con opciones de guardado DBF
                workbook.Save("DbfSaveOptionsDemo.dbf", saveOptions);
                
                Console.WriteLine("DBF file saved successfully with ExportAsString option set to true");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving DBF file: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [DbfSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


