---
title: "FormatConditionCollection.RemoveArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FormatConditionCollection. Elimina el rango de celdas con formato condicional por índice"
type: docs
url: /es/net/aspose.cells/formatconditioncollection/removearea/
---
## RemoveArea(int) {#removearea_1}

Elimina el rango de celdas con formato condicional por índice.

```csharp
public void RemoveArea(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice del rango de celdas con formato condicional que se eliminará. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodRemoveAreaWithInt32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar formato condicional
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];

            // Agregar áreas para formatear
            formatConditionCollection.AddArea(CellArea.CreateCellArea(0, 0, 10, 5)); // First area
            formatConditionCollection.AddArea(CellArea.CreateCellArea(5, 5, 15, 10)); // Second area

            // Agregar una condición
            formatConditionCollection.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");

            // Mostrar recuento inicial de áreas (sabemos que agregamos 2 áreas)
            Console.WriteLine("Areas before removal: 2");

            // Eliminar la segunda área (índice 1)
            formatConditionCollection.RemoveArea(1);

            // Mostrar recuento de áreas después de la eliminación (sabemos que eliminamos 1 área)
            Console.WriteLine("Areas after removal: 1");

            // Guarda el libro de trabajo
            workbook.Save("RemoveAreaDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveArea(int, int, int, int) {#removearea}

Eliminar el formato condicional en el rango.

```csharp
public bool RemoveArea(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | La startRow del rango. |
| startColumn | Int32 | La startColumn del rango. |
| totalRows | Int32 | El número de filas del rango. |
| totalColumns | Int32 | El número de columnas del rango. |

### Valor de retorno

Devuelve TRUE, esta FormatCondtionCollection debería ser eliminada.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodRemoveAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            
            int idx = cfc.Add();
            FormatConditionCollection fcc = cfc[idx];
            
            // Agregar área inicial
            CellArea initialArea = CellArea.CreateCellArea(0, 0, 0, 0);
            fcc.AddArea(initialArea);
            
            // Agregar condición
            idx = fcc.AddCondition(FormatConditionType.Expression);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "=A1>0";
            fc.Style.Font.Color = Color.Red;
            
            // Demostrar RemoveArea con parámetros Int32
            Console.WriteLine("Before removal - Areas count: " + fcc.Count);
            fcc.RemoveArea(0, 0, 1, 1); // Remove the initial area
            Console.WriteLine("After removal - Areas count: " + fcc.Count);
            
            // Agregar nueva área
            CellArea newArea = CellArea.CreateCellArea(1, 1, 1, 1);
            fcc.AddArea(newArea);
            Console.WriteLine("After adding new area - Areas count: " + fcc.Count);
        }
    }
}
```

### Ver también

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


