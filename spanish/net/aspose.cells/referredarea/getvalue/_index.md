---
title: "ReferredArea.GetValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ReferredArea. Obtiene el valor de la celda con el desplazamiento dado desde la esquina superior izquierda de esta área"
type: docs
url: /es/net/aspose.cells/referredarea/getvalue/
---
## GetValue(int, int) {#getvalue}

Obtiene el valor de la celda con el desplazamiento dado desde la esquina superior izquierda de esta área.

```csharp
public object GetValue(int rowOffset, int colOffset)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowOffset | Int32 | desplazamiento de fila desde la fila inicial de esta área |
| colOffset | Int32 | desplazamiento de columna desde la fila inicial de esta área |

### Valor de retorno

"#REF!" si esta área es inválida; "#N/A" si el desplazamiento dado está fuera de esta área; de lo contrario, devuelve el valor de la celda en la posición indicada.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaMethodGetValueWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue(5);
            Cell cell = worksheet.Cells["C1"];
            cell.Formula = "=A1";
            
            workbook.CalculateFormula();
            
            ReferredAreaCollection referredAreas = cell.GetPrecedents();
            if (referredAreas.Count > 0)
            {
                object value = referredAreas[0].GetValue(0, 0);
                Console.WriteLine("Value at (0,0): " + value);
            }
        }
    }
}
```

### Ver también

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetValue(int, int, bool) {#getvalue_1}

Obtiene el valor de la celda con el desplazamiento dado desde la esquina superior izquierda de esta área.

```csharp
public object GetValue(int rowOffset, int colOffset, bool calculateFormulas)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowOffset | Int32 | desplazamiento de fila desde la fila inicial de esta área |
| colOffset | Int32 | desplazamiento de columna desde la fila inicial de esta área |
| calculateFormulas | Booleano | Si calcularlo recursivamente cuando la referencia especificada es una fórmula |

### Valor de retorno

"#REF!" si esta área es inválida; "#N/A" si el desplazamiento dado está fuera de esta área; de lo contrario, devuelve el valor de la celda en la posición indicada.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaMethodGetValueWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue(100);
            sheet.Cells["B1"].PutValue(200);

            workbook.Worksheets.Names.Add("TestRange");
            Name name = workbook.Worksheets.Names["TestRange"];
            name.RefersTo = "=Sheet1!$A$1:$B$1";

            ReferredArea ra = name.GetReferredAreas(true)[0];
            object result = ra.GetValue(0, 0, true);

            Console.WriteLine("Obtained value: " + result);
        }
    }
}
```

### Ver también

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


