---
title: "LoadFilter.LoadFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "LoadFilter constructor. Construye un LoadFilter con las opciones de filtro predeterminadas LoadDataFilterOptions.All"
type: docs
url: /es/net/aspose.cells/loadfilter/loadfilter/
---
## LoadFilter() {#constructor}

Construye un LoadFilter con las opciones de filtro predeterminadas LoadDataFilterOptions.All.

```csharp
public LoadFilter()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadFilterMethodCtorDemo
    {
        public static void Run()
        {
            // Crear un nuevo LoadFilter con el constructor predeterminado
            LoadFilter filter = new LoadFilter();
            
            // Crear opciones de carga y asignar el filtro
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LoadFilter = filter;
            
            // Cargar libro de trabajo con el filtro
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);
            
            // Demostrar el uso contando hojas de cálculo
            Console.WriteLine("Number of worksheets loaded: " + workbook.Worksheets.Count);
            
            // Mostrar datos de celdas filtradas (todas las celdas cargadas por defecto)
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Console.WriteLine($"Worksheet '{sheet.Name}' has {sheet.Cells.Count} cells");
            }
        }
    }
}
```

### Ver también

* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## LoadFilter(LoadDataFilterOptions) {#constructor_1}

Construye un LoadFilter con las opciones de filtro proporcionadas.

```csharp
public LoadFilter(LoadDataFilterOptions opts)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opciones | LoadDataFilterOptions | las opciones de filtro predeterminadas |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterMethodCtorWithLoadDataFilterOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Preparar datos para los parámetros del método (LoadDataFilterOptions)
            LoadDataFilterOptions filterOptions = LoadDataFilterOptions.CellData | LoadDataFilterOptions.Chart;

            try
            {
                // Llamar al método #ctor con los tipos de parámetros específicos
                LoadFilter loadFilter = new LoadFilter(filterOptions);

                // Procesar o mostrar el resultado
                Console.WriteLine("LoadFilter created successfully with LoadDataFilterOptions: " + filterOptions);

                // Mostrar el efecto de la llamada al método
                Console.WriteLine("LoadDataFilterOptions set to: " + loadFilter.LoadDataFilterOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating LoadFilter: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("LoadFilterCtorWithLoadDataFilterOptionsDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [LoadDataFilterOptions](../../loaddatafilteroptions/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


