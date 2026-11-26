---
title: "LoadFilter.StartSheet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método LoadFilter. Prepara las opciones de filtro antes de cargar la hoja de cálculo dada. La implementación del usuario de LoadFilter puede cambiar el LoadDataFilterOptions aquí para indicar cómo cargar los datos para esta hoja de cálculo"
type: docs
url: /es/net/aspose.cells/loadfilter/startsheet/
---
## LoadFilter.StartSheet method

Prepara las opciones de filtro antes de cargar la hoja de cálculo dada. La implementación del usuario de LoadFilter puede cambiar las LoadDataFilterOptions aquí para indicar cómo cargar los datos para esta hoja de cálculo.

```csharp
public virtual void StartSheet(Worksheet sheet)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| hoja | Hoja de cálculo | La hoja de cálculo que se cargará. Sólo se pueden usar unas pocas propiedades para el objeto de hoja de cálculo dado aquí porque la mayoría de los datos y propiedades no se han cargado. Las propiedades disponibles son: Name, Index, VisibilityType |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterMethodStartSheetWithWorksheetDemo
    {
        // Crear una clase de filtro de carga personalizada que extienda LoadFilter
        class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
                Console.WriteLine($"Processing sheet: {sheet.Name}");
                // Puedes agregar lógica personalizada aquí para manejar hojas específicas
            }
        }

        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "TestSheet";

            // Crear una instancia de nuestro filtro de carga personalizado
            CustomLoadFilter loadFilter = new CustomLoadFilter();

            try
            {
                // Llamar al método StartSheet con el parámetro worksheet
                loadFilter.StartSheet(worksheet);
                
                Console.WriteLine("StartSheet method executed successfully");
                
                // Agregar algunos datos para demostrar que la hoja es accesible
                worksheet.Cells["A1"].PutValue("StartSheet Demo");
                worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartSheet method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("LoadFilterStartSheetDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../../worksheet/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


