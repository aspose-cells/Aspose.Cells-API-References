---
title: "ListObject.PutCellValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ListObject. Asigna el valor a la celda"
type: docs
url: /es/net/aspose.cells.tables/listobject/putcellvalue/
---
## PutCellValue(int, int, object) {#putcellvalue}

Coloca el valor en la celda.

```csharp
public void PutCellValue(int rowOffset, int columnOffset, object value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowOffset | Int32 | El desplazamiento de fila en la tabla. |
| columnOffset | Int32 | El desplazamiento de columna en la tabla. |
| valor | Objeto | El valor de la celda. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellValueWithInt32Int32ObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de ejemplo
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["C1"].PutValue("Column3");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["C2"].PutValue(300);

            // Crear un objeto de lista
            int index = worksheet.ListObjects.Add(0, 0, 2, 2, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Demostrar PutCellValue con parámetros Int32, Int32, Object
            listObject.PutCellValue(1, 0, 500); // Update row 1, column 0 with value 500
            listObject.PutCellValue(1, 1, "Updated Value"); // Update row 1, column 1 with string
            listObject.PutCellValue(1, 2, DateTime.Now); // Update row 1, column 2 with current date

            // Guarda el libro de trabajo
            workbook.Save("ListObjectPutCellValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## PutCellValue(int, int, object, bool) {#putcellvalue_1}

Coloca el valor en la celda.

```csharp
public void PutCellValue(int rowOffset, int columnOffset, object value, bool isTotalsRowLabel)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowOffset | Int32 | El desplazamiento de fila en la tabla. |
| columnOffset | Int32 | El desplazamiento de columna en la tabla. |
| valor | Objeto | El valor de la celda. |
| isTotalsRowLabel | Booleano | Indica si es una etiqueta para la fila total, solo funciona para la fila total. Si es False y esta fila es la fila total, se insertará una nueva fila. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellValueWithInt32Int32ObjectBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para crear un ListObject
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");
            
            // Crear un ListObject
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // Usar PutCellValue para actualizar una celda (fila 2, columna 1) con un nuevo valor y expandir la tabla
            listObject.PutCellValue(2, 1, "Updated Value", true);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


