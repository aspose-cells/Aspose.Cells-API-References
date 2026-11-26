---
title: "UnknownControl.GetRelationshipData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método UnknownControl. Obtiene los datos relacionados"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/unknowncontrol/getrelationshipdata/
---
## UnknownControl.GetRelationshipData method

Obtiene los datos relacionados.

```csharp
public byte[] GetRelationshipData(string relId)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| relId | String | El identificador de la relación. |

### Valor de retorno

Devuelve los datos relacionados.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class UnknownControlMethodGetRelationshipDataWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Intentar agregar un control ActiveX desconocido
            Shape shape;
            try
            {
                shape = worksheet.Shapes.AddActiveXControl(ControlType.Unknown, 0, 0, 0, 0, 100, 100);
            }
            catch (ArgumentException ex)
            {
                Console.WriteLine($"Could not create control: {ex.Message}");
                return;
            }

            // Obtener el control como UnknownControl
            UnknownControl unknownControl = shape.ActiveXControl as UnknownControl;
            if (unknownControl == null)
            {
                Console.WriteLine("ActiveX control is not UnknownControl type");
                return;
            }

            try
            {
                // Ejecutar GetRelationshipData con un parámetro de cadena
                string relationshipId = "rId1";
                byte[] relationshipData = unknownControl.GetRelationshipData(relationshipId);

                Console.WriteLine("GetRelationshipData executed successfully");
                Console.WriteLine(relationshipData == null 
                    ? "No relationship data found" 
                    : $"Received {relationshipData.Length} bytes of data");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("UnknownControlGetRelationshipDataDemo.xlsx");
        }
    }
}
```

### Ver también

* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


