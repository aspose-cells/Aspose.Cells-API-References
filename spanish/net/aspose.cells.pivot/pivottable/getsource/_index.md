---
title: "PivotTable.GetSource"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de PivotTable. Obtiene la fuente de datos de esta tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/getsource/
---
## GetSource() {#getsource}

Obtén la fuente de datos de esta tabla dinámica.

```csharp
public string[] GetSource()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetSourceDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Obtén y muestra el rango de datos de origen
            string[] sourceData = pivotTable.GetSource();
            Console.WriteLine("Pivot Table Source: " + sourceData[0]);
            
            // Cambia la fuente de datos
            pivotTable.ChangeDataSource(new[] { "A1:B4" });
            
            // Verifica la fuente modificada
            sourceData = pivotTable.GetSource();
            Console.WriteLine("Updated Pivot Table Source: " + sourceData[0]);
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GetSource(bool) {#getsource_1}

Obtén la fuente de datos de esta tabla dinámica.

```csharp
public string[] GetSource(bool isOriginal)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isOriginal | Booleano | Indica si se debe devolver la fuente original o la fuente de datos mostrada. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetSourceWithBooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("example.xlsx");
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accede a la primera tabla dinámica
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Obtén los datos de origen con ruta local (true)
            string[] localSource = pivotTable.GetSource(true);
            Console.WriteLine("Local path source: " + localSource[0]);
            
            // Obtén los datos de origen con ruta completa (false)
            string[] fullSource = pivotTable.GetSource(false);
            Console.WriteLine("Full path source: " + fullSource[0]);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


