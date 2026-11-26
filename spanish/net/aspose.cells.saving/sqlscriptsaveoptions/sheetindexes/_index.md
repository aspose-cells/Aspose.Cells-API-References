---
title: "SqlScriptSaveOptions.SheetIndexes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SqlScriptSaveOptions. Representa los índices de las hojas exportadas"
type: docs
url: /es/net/aspose.cells.saving/sqlscriptsaveoptions/sheetindexes/
---
## SqlScriptSaveOptions.SheetIndexes property

Representa los índices de las hojas exportadas.

```csharp
public int[] SheetIndexes { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SqlScriptSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con varias hojas
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Poblar algunos datos en todas las hojas
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet worksheet = workbook.Worksheets[i];
                worksheet.Cells["A1"].PutValue("ID");
                worksheet.Cells["B1"].PutValue("Name");
                worksheet.Cells["A2"].PutValue(1);
                worksheet.Cells["B2"].PutValue("John");
                worksheet.Cells["A3"].PutValue(2);
                worksheet.Cells["B3"].PutValue("Jane");
            }

            // Crear una instancia de SqlScriptSaveOptions
            SqlScriptSaveOptions options = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                CreateTable = true,
                HasHeaderRow = true
            };

            // Mostrar los SheetIndexes actuales (null significa todas las hojas)
            Console.WriteLine("Initial SheetIndexes: " + 
                (options.SheetIndexes == null ? "All sheets" : string.Join(",", options.SheetIndexes)));

            // Establecer SheetIndexes para exportar solo la primera y tercera hoja (0 y 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // Guardar con las opciones
            workbook.Save("SqlScriptExportSelectedSheets.sql", options);

            // Cambiar SheetIndexes para exportar solo la segunda hoja
            options.SheetIndexes = new int[] { 1 };
            workbook.Save("SqlScriptExportSecondSheet.sql", options);

            // Establecer SheetIndexes a nulo para exportar todas las hojas
            options.SheetIndexes = null;
            workbook.Save("SqlScriptExportAllSheets.sql", options);
        }
    }
}
```

### Ver también

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


