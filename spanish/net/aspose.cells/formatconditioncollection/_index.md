---
title: "Clase FormatConditionCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.FormatConditionCollection. Representa el formato condicional. Los FormatConditions pueden contener hasta tres formatos condicionales"
type: docs
url: /es/net/aspose.cells/formatconditioncollection/
---
## FormatConditionCollection class

Representa el formato condicional. Las FormatConditions pueden contener hasta tres formatos condicionales.

```csharp
public class FormatConditionCollection
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.cells/formatconditioncollection/count/) { get; } | Obtiene el recuento de las condiciones. |
| [Item](../../aspose.cells/formatconditioncollection/item/) { get; } | Obtiene la condición de formato por índice. |
| [RangeCount](../../aspose.cells/formatconditioncollection/rangecount/) { get; } | Obtiene el recuento de rangos con formato condicional. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells/formatconditioncollection/add/)(CellArea, FormatConditionType, OperatorType, string, string) | Agrega una condición de formato y el rango de celdas afectado a los FormatConditions. Los FormatConditions pueden contener hasta tres formatos condicionales. No se permiten referencias a otras hojas en las fórmulas del formato condicional. |
| [AddArea](../../aspose.cells/formatconditioncollection/addarea/)(CellArea) | Agrega un rango de celdas con formato condicional. |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition/#addcondition)(FormatConditionType) | Agregar una condición de formato. |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition/#addcondition_1)(FormatConditionType, OperatorType, string, string) | Agrega una condición de formato. |
| [GetCellArea](../../aspose.cells/formatconditioncollection/getcellarea/)(int) | Obtiene el rango de celdas con formato condicional por índice. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea/#removearea_1)(int) | Elimina el rango de celdas con formato condicional por índice. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea/#removearea)(int, int, int, int) | Eliminar el formato condicional en el rango. |
| [RemoveCondition](../../aspose.cells/formatconditioncollection/removecondition/)(int) | Elimina la condición de formato por índice. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionCollectionDemo
    {
        public static void FormatConditionCollectionExample()
        {
            // Crear un nuevo Workbook
            Workbook workbook = new Workbook();

            // Obtener la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];

            // Agrega un formato condicional vacío
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Establece el rango de formato condicional
            CellArea ca = new CellArea { StartRow = 0, EndRow = 0, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);
            ca = new CellArea { StartRow = 1, EndRow = 1, StartColumn = 1, EndColumn = 1 };
            fcs.AddArea(ca);

            // Agrega condiciones
            int conditionIndex1 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");

            // Establece el color de fondo
            FormatCondition fc1 = fcs[conditionIndex1];
            fc1.Style.BackgroundColor = System.Drawing.Color.Red;

            // Guardando el archivo Excel
            workbook.Save("FormatConditionCollectionExample.xlsx");
            workbook.Save("FormatConditionCollectionExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


