---
title: "WorksheetCollection.SensitivityLabels"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorksheetCollection. Representa todas las etiquetas de sensibilidad"
type: docs
url: /es/net/aspose.cells/worksheetcollection/sensitivitylabels/
---
## WorksheetCollection.SensitivityLabels property

Representa todas las etiquetas de sensibilidad.

```csharp
public SensitivityLabelCollection SensitivityLabels { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metas;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertySensitivityLabelsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la colección de hojas de cálculo
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Agregar una etiqueta de sensibilidad
            int index = worksheets.SensitivityLabels.Add(
                "{7e848398-70bd-400c-b8cf-2ab6f30d1b60}", // ID
                true,                                       // IsEnabled
                SensitivityLabelAssignmentType.Standard,     // AssignmentType
                "contoso-site",                             // SiteId
                SensitivityLabelMarkType.Header              // MarkType
            );
            
            // Verificar la etiqueta agregada
            SensitivityLabel label = worksheets.SensitivityLabels[index];
            Console.WriteLine($"Label added - ID: {label.Id}, SiteID: {label.SiteId}");
            
            // Guarda el libro de trabajo
            workbook.Save("SensitivityLabelsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SensitivityLabelCollection](../../../aspose.cells.metas/sensitivitylabelcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


