---
title: "UnknownControl.GetRelationshipData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo UnknownControl. Ottiene i dati correlati"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/unknowncontrol/getrelationshipdata/
---
## UnknownControl.GetRelationshipData method

Ottiene i dati correlati.

```csharp
public byte[] GetRelationshipData(string relId)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| relId | String | L'ID della relazione. |

### Valore di ritorno

Restituisce i dati correlati.

### Esempi

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

            // Tentativo di aggiungere un controllo ActiveX sconosciuto
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

            // Ottieni il controllo come UnknownControl
            UnknownControl unknownControl = shape.ActiveXControl as UnknownControl;
            if (unknownControl == null)
            {
                Console.WriteLine("ActiveX control is not UnknownControl type");
                return;
            }

            try
            {
                // Esegui GetRelationshipData con parametro stringa
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

### Vedi anche

* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


