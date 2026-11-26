---
title: "LoadFilter.LoadDataFilterOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadFilter. Las opciones de filtro para indicar qué datos deben cargarse"
type: docs
url: /es/net/aspose.cells/loadfilter/loaddatafilteroptions/
---
## LoadFilter.LoadDataFilterOptions property

Las opciones de filtro para indicar qué datos deben cargarse.

```csharp
public LoadDataFilterOptions LoadDataFilterOptions { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterPropertyLoadDataFilterOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = 123;
            worksheet.Cells["C1"].Formula = "=SUM(A1:B1)";

            try
            {
                // Crear una instancia de LoadFilter con opciones predeterminadas
                LoadFilter loadFilter = new LoadFilter();

                // Mostrar el valor predeterminado de LoadDataFilterOptions
                Console.WriteLine("Default LoadDataFilterOptions: " + loadFilter.LoadDataFilterOptions);

                // Establecer nuevas opciones de filtro (combinación de banderas)
                loadFilter.LoadDataFilterOptions = LoadDataFilterOptions.CellValue | LoadDataFilterOptions.Formula;

                // Mostrar el valor actualizado
                Console.WriteLine("Updated LoadDataFilterOptions: " + loadFilter.LoadDataFilterOptions);

                // Crear otro filtro con opciones diferentes
                LoadFilter anotherFilter = new LoadFilter(LoadDataFilterOptions.Chart | LoadDataFilterOptions.Picture);

                // Mostrar las opciones del constructor
                Console.WriteLine("Constructor LoadDataFilterOptions: " + anotherFilter.LoadDataFilterOptions);

                // Guarda el libro de trabajo
                workbook.Save("LoadDataFilterOptionsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* enum [LoadDataFilterOptions](../../loaddatafilteroptions/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


