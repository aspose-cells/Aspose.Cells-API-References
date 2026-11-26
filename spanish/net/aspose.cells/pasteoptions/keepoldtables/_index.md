---
title: "PasteOptions.KeepOldTables"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PasteOptions. Mantiene las tablas en el rango de destino"
type: docs
url: /es/net/aspose.cells/pasteoptions/keepoldtables/
---
## PasteOptions.KeepOldTables property

Mantiene las tablas en el rango de destino.

```csharp
public bool KeepOldTables { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PasteOptionsPropertyKeepOldTablesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Crear una hoja de cálculo de ejemplo con datos
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Source Data";
            worksheet.Cells["B1"].Value = "Table Data";

            try
            {
                // Crear una instancia de PasteOptions
                PasteOptions pasteOptions = new PasteOptions();

                // Mostrar el valor predeterminado de la propiedad KeepOldTables
                Console.WriteLine("Default KeepOldTables value: " + pasteOptions.KeepOldTables);

                // Establecer KeepOldTables en true
                pasteOptions.KeepOldTables = true;
                Console.WriteLine("KeepOldTables set to: " + pasteOptions.KeepOldTables);

                // Crear rangos para la operación de copia
                Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:B1");
                Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("A3:B3");

                // Copiar con la opción KeepOldTables
                targetRange.Copy(sourceRange, pasteOptions);

                // Guarda el libro de trabajo
                workbook.Save("KeepOldTablesDemo.xlsx");
                Console.WriteLine("Workbook saved with KeepOldTables option applied.");
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

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


