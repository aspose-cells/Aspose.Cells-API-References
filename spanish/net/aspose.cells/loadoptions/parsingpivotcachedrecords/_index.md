---
title: "LoadOptions.ParsingPivotCachedRecords"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Indica si se analizan los registros en caché de tablas dinámicas al cargar el archivo. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/loadoptions/parsingpivotcachedrecords/
---
## LoadOptions.ParsingPivotCachedRecords property

Indica si se analizan los registros en caché de la tabla dinámica al cargar el archivo. El valor predeterminado es false.

```csharp
public bool ParsingPivotCachedRecords { get; set; }
```

### Observaciones

Solo se aplica a archivos Excel Xlsx, Xltx, Xltm, Xlsm y xlsb

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyParsingPivotCachedRecordsDemo
    {
        public static void Run()
        {
            // Crear opciones de carga CSV
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
            
            // Habilitar el análisis de registros en caché de tablas dinámicas
            loadOptions.ParsingPivotCachedRecords = true;
            
            // Cargue el libro de trabajo con las opciones
            Workbook workbook = new Workbook("example.csv", loadOptions);
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "PivotData";
            
            // Crear tabla dinámica (demostrando que la propiedad está configurada)
            int pivotIndex = worksheet.PivotTables.Add("A1:C10", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableOutput.xlsx");
        }
    }
}
```

### Ver también

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


