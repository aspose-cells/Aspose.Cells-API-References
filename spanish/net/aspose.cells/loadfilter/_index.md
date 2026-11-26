---
title: "Clase LoadFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.LoadFilter. Representa el filtro que proporciona opciones para cargar datos al cargar el libro de trabajo desde una plantilla"
type: docs
url: /es/net/aspose.cells/loadfilter/
---
## LoadFilter class

Representa el filtro que brinda opciones para cargar datos al cargar el libro de trabajo desde una plantilla.

```csharp
public class LoadFilter
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [LoadFilter](loadfilter/#constructor)() | Construye un LoadFilter con las opciones de filtro predeterminadas LoadDataFilterOptions.All. |
| [LoadFilter](loadfilter/#constructor_1)(LoadDataFilterOptions) | Construye un LoadFilter con las opciones de filtro proporcionadas. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [LoadDataFilterOptions](../../aspose.cells/loadfilter/loaddatafilteroptions/) { get; set; } | Las opciones de filtro para indicar qué datos deben cargarse. |
| virtual [SheetsInLoadingOrder](../../aspose.cells/loadfilter/sheetsinloadingorder/) { get; } | Especifica las hojas (índices) y el orden que se cargarán. El valor predeterminado es null, lo que indica cargar todas las hojas en el orden predeterminado del archivo de plantilla. Si no es null y el índice de alguna hoja no está en la matriz devuelta, entonces esa hoja no se cargará. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [StartSheet](../../aspose.cells/loadfilter/startsheet/)(Worksheet) | Prepara las opciones de filtro antes de cargar la hoja de cálculo dada. La implementación del usuario de LoadFilter puede cambiar las LoadDataFilterOptions aquí para indicar cómo cargar los datos para esta hoja de cálculo. |

### Observaciones

El usuario puede especificar las opciones de filtro o implementar su propio LoadFilter para indicar cómo cargar los datos.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterDemo
    {
        public static void LoadFilterExample()
        {
            // Crear LoadOptions y establecer LoadFilter
            LoadOptions opts = new LoadOptions();
            opts.LoadFilter = new CustomLoadFilter();

            // Cargar el libro de trabajo con los LoadOptions especificados
            Workbook wb = new Workbook("LoadFilterExample_original.xlsx", opts);

            // Guardar el libro de trabajo para ver el efecto de LoadFilter
            wb.Save("LoadFilterExample.xlsx");
        }

        // Implementación personalizada de LoadFilter
        public class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
                if (sheet.Name == "Sheet1")
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.All;
                }
                else
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.Structure;
                }
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


