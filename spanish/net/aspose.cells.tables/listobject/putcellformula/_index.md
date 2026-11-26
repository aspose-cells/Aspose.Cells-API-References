---
title: "ListObject.PutCellFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de ListObject. Coloca la fórmula en la celda de la tabla"
type: docs
url: /es/net/aspose.cells.tables/listobject/putcellformula/
---
## PutCellFormula(int, int, string) {#putcellformula}

Coloca la fórmula en la celda de la tabla.

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowOffset | Int32 | El desplazamiento de fila en la tabla. |
| columnOffset | Int32 | El desplazamiento de columna en la tabla. |
| fórmula | String | La fórmula de la celda. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellFormulaWithInt32Int32StringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Agregar datos de ejemplo para crear una tabla
            sheet.Cells["A1"].PutValue("ID");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["C1"].PutValue("Formula");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["B3"].PutValue(20);

            // Crear un objeto lista (tabla)
            int index = sheet.ListObjects.Add("A1", "C3", true);
            ListObject table = sheet.ListObjects[index];

            // Agregar una nueva fila y establecer valores/fórmula
            table.PutCellValue(4, 0, 3); // Row 4, Column 0 (ID)
            table.PutCellValue(4, 1, 30); // Row 4, Column 1 (Value)
            table.PutCellFormula(4, 2, "=B3*2"); // Row 4, Column 2 (Formula)

            // Guarda el libro de trabajo
            wb.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## PutCellFormula(int, int, string, bool) {#putcellformula_1}

Coloca la fórmula en la celda de la tabla.

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula, bool isTotalsRowFormula)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowOffset | Int32 | El desplazamiento de fila en la tabla. |
| columnOffset | Int32 | El desplazamiento de columna en la tabla. |
| fórmula | String | La fórmula de la celda. |
| isTotalsRowFormula | Booleano |  |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellFormulaWithInt32Int32StringBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregue datos de ejemplo para crear un objeto de lista
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            
            // Crear objeto de lista
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // Demostrar PutCellFormula
            listObject.PutCellFormula(3, 0, "=SUM(A2:A3)", true);
            
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


