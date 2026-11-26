---
title: "Validation.AddArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Validation. Aplica la validación al área"
type: docs
url: /es/net/aspose.cells/validation/addarea/
---
## AddArea(CellArea) {#addarea}

Aplica la validación al área.

```csharp
public void AddArea(CellArea cellArea)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellArea | CellArea | El área. |

### Observaciones

Es equivalente usar `AddArea` con verificación de intersección y borde.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodAddAreaWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Crear una validación
            ValidationCollection vc = sheet.Validations;
            Validation validation = vc[vc.Add(CellArea.CreateCellArea(0, 0, 0, 0))];
            validation.Type = ValidationType.List;
            validation.Formula1 = "=A1:A10";

            // Agregar más áreas a la validación
            for (int i = 1; i < 5; i++)
            {
                validation.AddArea(CellArea.CreateCellArea(i, 0, i, 0));
            }

            // Guarda el libro de trabajo
            wb.Save("ValidationMethodAddAreaWithCellAreaDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Validation with multiple areas created successfully.");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddArea(CellArea, bool, bool) {#addarea_1}

Aplica la validación al área.

```csharp
public void AddArea(CellArea cellArea, bool checkIntersection, bool checkEdge)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellArea | CellArea | El área. |
| checkIntersection | Booleano | Indica si se verifica la intersección del área dada con las áreas de validaciones existentes. Si una validación ha sido aplicada en el área dada (o en parte de ella), entonces la validación existente debe eliminarse primero del área dada. De lo contrario, podría producirse corrupción en las validaciones generadas. Si el usuario está seguro de que el área añadida no intersecta con ninguna área existente, este parámetro puede establecerse en false por consideraciones de rendimiento. |
| checkEdge | Booleano | Indica si se verifica el borde de las áreas aplicadas de esta validación. La configuración interna de Validation depende del área superior‑izquierda de sus rangos aplicados, por lo que si el área dada se convierte en la nueva superior‑izquierda de los rangos aplicados, la configuración interna debe modificarse y reconstruirse; de lo contrario, pueden producirse resultados inesperados. Si el usuario está seguro de que el área añadida no es la superior‑izquierda, este parámetro puede establecerse en false por consideraciones de rendimiento. |

### Observaciones

En este método, eliminaremos todas las validaciones antiguas en el área dada. Para el rango superior‑izquierda de los rangos aplicados de Validation, primero su StartRow es el más pequeño, segundo su StartColumn es el más pequeño entre aquellas áreas que comparten el mismo StartRow mínimo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodAddAreaWithCellAreaBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una validación en un área específica
            Validation validation = worksheet.Validations[worksheet.Validations.Add(CellArea.CreateCellArea(5, 3, 6, 3))];
            validation.Operator = OperatorType.GreaterThan;
            validation.Formula1 = "F3";

            // Demostrar AddArea con CellArea y dos parámetros booleanos
            validation.AddArea(CellArea.CreateCellArea(3, 3, 3, 4), false, true);
            Console.WriteLine("Area count after AddArea: " + validation.Areas.Length);
            Console.WriteLine("Formula1 after AddArea: " + validation.Formula1);

            // Eliminar el área añadida
            validation.RemoveArea(CellArea.CreateCellArea(3, 3, 3, 4));
            Console.WriteLine("Area count after RemoveArea: " + validation.Areas.Length);

            // Agregar múltiples áreas con una operación masiva
            CellArea[] areas = new CellArea[10];
            for (int i = 0; i < areas.Length; i++)
            {
                areas[i] = CellArea.CreateCellArea(6 + i, 3, 6 + i, 4);
            }
            validation.AddAreas(areas, true, true);
            Console.WriteLine("Area count after bulk AddAreas: " + validation.Areas.Length);

            // Guarda el libro de trabajo
            workbook.Save("ValidationMethodAddAreaDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


