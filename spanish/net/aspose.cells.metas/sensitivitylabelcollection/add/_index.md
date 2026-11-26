---
title: "SensitivityLabelCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SensitivityLabelCollection. Añade una etiqueta de sensibilidad"
type: docs
url: /es/net/aspose.cells.metas/sensitivitylabelcollection/add/
---
## SensitivityLabelCollection.Add method

Añade una etiqueta de sensibilidad.

```csharp
public int Add(string id, bool isEnabled, SensitivityLabelAssignmentType methodType, string siteId, 
    SensitivityLabelMarkType markType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| id | String | El id de la etiqueta. |
| isEnabled | Booleano | Indica si esta etiqueta de sensibilidad está habilitada. |
| methodType | SensitivityLabelAssignmentType | El tipo de método de asignación. |
| siteId | String | El id del sitio. |
| markType | SensitivityLabelMarkType | El tipo de marca. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelCollectionMethodAddWithStringBooleanSensitivityLabelADemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Cree una nueva SensitivityLabelCollection
            var sensitivityLabels = new SensitivityLabelCollection();
            
            try
            {
                // Llame al método Add con parámetros específicos
                int index = sensitivityLabels.Add(
                    id: "Confidential",
                    isEnabled: true,
                    methodType: SensitivityLabelAssignmentType.Privileged,
                    siteId: "Contoso",
                    markType: SensitivityLabelMarkType.Watermark);
                
                Console.WriteLine($"Sensitivity label added at index: {index}");
                
                // Añada algunos datos para demostrar el efecto
                worksheet.Cells["A1"].Value = "Confidential Data";
                worksheet.Cells["A2"].Value = "This document contains sensitive information";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("SensitivityLabelAddDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [SensitivityLabelAssignmentType](../../sensitivitylabelassignmenttype/)
* enum [SensitivityLabelMarkType](../../sensitivitylabelmarktype/)
* class [SensitivityLabelCollection](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


