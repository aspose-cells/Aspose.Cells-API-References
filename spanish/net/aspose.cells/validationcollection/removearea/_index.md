---
title: "ValidationCollection.RemoveArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ValidationCollection. Elimina todas las configuraciones de validación en el rango"
type: docs
url: /es/net/aspose.cells/validationcollection/removearea/
---
## ValidationCollection.RemoveArea method

Elimina todas las configuraciones de validación en el rango..

```csharp
public void RemoveArea(CellArea ca)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | CellArea | El rango que contiene la configuración de validaciones. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationCollectionMethodRemoveAreaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear una validación en un área específica
            ValidationCollection validations = worksheet.Validations;
            CellArea validationArea = CellArea.CreateCellArea(0, 0, 5, 5);
            int validationIndex = validations.Add(validationArea);
            
            // Crear un área para eliminar de la validación
            CellArea removeArea = CellArea.CreateCellArea(2, 2, 4, 4);
            
            try
            {
                // Llamar al método RemoveArea con el parámetro CellArea
                validations.RemoveArea(removeArea);
                
                Console.WriteLine("Validation area removed successfully.");
                
                // Mostrar las áreas de validación restantes
                foreach (Validation validation in validations)
                {
                    if (validation.Areas.Length > 0)
                    {
                        Console.WriteLine($"Remaining validation area: {validation.Areas[0]}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveArea method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("ValidationRemoveAreaDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


