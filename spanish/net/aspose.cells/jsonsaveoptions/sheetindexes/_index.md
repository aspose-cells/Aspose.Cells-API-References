---
title: "JsonSaveOptions.SheetIndexes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonSaveOptions. Representa los índices de las hojas exportadas"
type: docs
url: /es/net/aspose.cells/jsonsaveoptions/sheetindexes/
---
## JsonSaveOptions.SheetIndexes property

Representa los índices de las hojas exportadas.

```csharp
public int[] SheetIndexes { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class JsonSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con varias hojas
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Poblar algunos datos en cada hoja
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue($"Data from Sheet {i + 1}");
            }

            // Crear una instancia de JsonSaveOptions
            JsonSaveOptions options = new JsonSaveOptions();

            // Mostrar los SheetIndexes actuales (null por defecto - exporta todas las hojas)
            Console.WriteLine("Current SheetIndexes: " + (options.SheetIndexes == null ? "Exporting all sheets" : string.Join(",", options.SheetIndexes)));

            // Configurar para exportar solo la primera y la tercera hoja (índices 0 y 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // Guardar a JSON con hojas seleccionadas
            workbook.Save("JsonSaveOptionsPropertySheetIndexesDemo.json", options);

            // Verificar cargando el JSON
            string jsonContent = System.IO.File.ReadAllText("JsonSaveOptionsPropertySheetIndexesDemo.json");
            Console.WriteLine("JSON Content:");
            Console.WriteLine(jsonContent);

            // Cambiar para exportar solo la segunda hoja (índice 1)
            options.SheetIndexes = new int[] { 1 };
            workbook.Save("JsonSaveOptionsPropertySheetIndexesDemo_SingleSheet.json", options);

            // Verificar la exportación de una sola hoja
            jsonContent = System.IO.File.ReadAllText("JsonSaveOptionsPropertySheetIndexesDemo_SingleSheet.json");
            Console.WriteLine("Single Sheet JSON Content:");
            Console.WriteLine(jsonContent);
        }
    }
}
```

### Ver también

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


