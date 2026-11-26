---
title: "Validation.AddAreas"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Validation. Aplica la validación a las áreas dadas"
type: docs
url: /es/net/aspose.cells/validation/addareas/
---
## Validation.AddAreas method

Aplica la validación a las áreas dadas.

```csharp
public void AddAreas(CellArea[] areas, bool checkIntersection, bool checkEdge)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| áreas | CellArea[] | Las áreas. |
| checkIntersection | Booleano | Si se verifica la intersección del área dada con las áreas de validaciones existentes. Si una validación se ha aplicado en el área dada (o parte de ella), entonces la validación existente debe eliminarse primero del área dada. De lo contrario, puede producirse corrupción en las Validaciones generadas. Si el usuario está seguro de que todas las áreas añadidas no intersectan con ninguna área existente, este parámetro puede establecerse como false por consideraciones de rendimiento. |
| checkEdge | Booleano | Si se verifica el borde de las áreas aplicadas de esta validación. La configuración interna de la Validación depende de la zona superior‑izquierda de sus rangos aplicados, por lo que si una de las áreas dadas llega a ser la nueva zona superior‑izquierda de los rangos aplicados, la configuración interna debe cambiarse y reconstruirse; de lo contrario, se pueden producir resultados inesperados. Si el usuario está seguro de que ninguna de esas áreas añadidas es la superior‑izquierda, este parámetro puede establecerse como false por consideraciones de rendimiento. |

### Observaciones

En este método, eliminaremos todas las validaciones antiguas en el área dada. Para el rango superior‑izquierda de los rangos aplicados de Validation, primero su StartRow es el más pequeño, segundo su StartColumn es el más pequeño entre aquellas áreas que comparten el mismo StartRow mínimo.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodAddAreasWithCellAreaBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int validationIndex = worksheet.Validations.Add();
            Validation validation = worksheet.Validations[validationIndex];
            validation.Type = ValidationType.List;
            validation.AlertStyle = ValidationAlertType.Stop;
            validation.Operator = OperatorType.None;
            validation.Formula1 = "1,2,3";
            validation.InCellDropDown = true;

            CellArea[] areas = new CellArea[2];
            areas[0] = new CellArea { StartRow = 0, StartColumn = 0, EndRow = 1, EndColumn = 1 };
            areas[1] = new CellArea { StartRow = 2, StartColumn = 2, EndRow = 3, EndColumn = 3 };

            try
            {
                validation.AddAreas(areas, true, false);
                Console.WriteLine("Added validation areas with checkIntersection=true, checkEdge=false");

                foreach (CellArea area in validation.Areas)
                {
                    Console.WriteLine($"Validation area: R{area.StartRow + 1}C{area.StartColumn + 1}:R{area.EndRow + 1}C{area.EndColumn + 1}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding validation areas: {ex.Message}");
            }

            workbook.Save("ValidationAddAreasDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


