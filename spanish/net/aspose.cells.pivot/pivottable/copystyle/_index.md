---
title: "PivotTable.CopyStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de PivotTable. Copia el estilo nombrado de otra tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/copystyle/
---
## PivotTable.CopyStyle method

Copia el estilo con nombre de otra tabla dinámica.

```csharp
public void CopyStyle(PivotTable pivotTable)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivotTable | PivotTable | Tabla dinámica de origen. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCopyStyleWithPivotTableDemo
    {
        public static void Run()
        {
            // Crear libro de origen con tabla dinámica
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            sourceSheet.Cells["A1"].PutValue("Product");
            sourceSheet.Cells["B1"].PutValue("Sales");
            sourceSheet.Cells["A2"].PutValue("A");
            sourceSheet.Cells["B2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue("B");
            sourceSheet.Cells["B3"].PutValue(200);
            
            // Crear tabla dinámica de origen (obtener explícitamente el objeto de la tabla dinámica)
            PivotTable sourcePivotTable = sourceSheet.PivotTables[sourceSheet.PivotTables.Add("PivotTable1", "A1:B3", "C3")];
            sourcePivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            sourcePivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Aplicar estilo a la tabla dinámica de origen
            sourcePivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            
            // Crear libro de destino con tabla dinámica
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Agregar la misma estructura de datos
            destSheet.Cells["A1"].PutValue("Product");
            destSheet.Cells["B1"].PutValue("Sales");
            destSheet.Cells["A2"].PutValue("A");
            destSheet.Cells["B2"].PutValue(150);
            destSheet.Cells["A3"].PutValue("B");
            destSheet.Cells["B3"].PutValue(250);
            
            // Crear tabla dinámica de destino (obtener explícitamente el objeto de la tabla dinámica)
            PivotTable destPivotTable = destSheet.PivotTables[destSheet.PivotTables.Add("PivotTable2", "A1:B3", "C3")];
            destPivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            destPivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Copiar estilo del origen a la tabla dinámica de destino
            destPivotTable.CopyStyle(sourcePivotTable);
            
            // Guardar el resultado
            destWorkbook.Save("PivotTableStyleCopied.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


