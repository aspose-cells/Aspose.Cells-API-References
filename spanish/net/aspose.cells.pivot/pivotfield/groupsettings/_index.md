---
title: "PivotField.GroupSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Obtiene la configuración de agrupación del pivot field"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/groupsettings/
---
## PivotField.GroupSettings property

Obtiene la configuración de grupo del campo de tabla dinámica.

```csharp
public PivotFieldGroupSettings GroupSettings { get; }
```

### Observaciones

Si este campo no está agrupado, se devolverá Null.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyGroupSettingsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("example.xlsx");
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accede a la primera tabla dinámica
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Acceda al segundo campo base (suponiendo que exista)
            if (pivotTable.BaseFields.Count > 1)
            {
                PivotField pivotField = pivotTable.BaseFields[1];
                
                // Verifique si el campo tiene configuraciones de agrupación
                if (pivotField.GroupSettings != null)
                {
                    Console.WriteLine("Field has grouping enabled");
                    Console.WriteLine("Group type: " + pivotField.GroupSettings.Type);
                }
                else
                {
                    Console.WriteLine("Field has no grouping settings");
                }
                
                // Ejemplo de agrupación de un campo numérico
                if (pivotField.GroupSettings == null && 
                    pivotField.PivotItems.Count > 0 && 
                    pivotField.PivotItems[0].Value is double)
                {
                    // Agrupar por rango numérico (intervalos de 10 unidades)
                    pivotField.GroupBy(10.0, false);
                    Console.WriteLine("Field grouped by numeric range");
                }
            }
            
            // Guardar el libro de trabajo modificado
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFieldGroupSettings](../../pivotfieldgroupsettings/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


