---
title: "UnknownControl.Data"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà UnknownControl. Ottiene e imposta i dati binari del controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/unknowncontrol/data/
---
## UnknownControl.Data property

Ottiene e imposta i dati binari del controllo.

```csharp
public override byte[] Data { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class UnknownControlPropertyDataDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un CLSID fittizio (identificatore non valido)
            byte[] dummyClsid = new byte[16];

            // Aggiungi un controllo ActiveX sconosciuto usando ControlType.Unknown con tutti i parametri
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Unknown, 0, 0, 100, 100, 0, 0);

            // Accedi all'istanza UnknownControl
            UnknownControl unknownControl = (UnknownControl)shape.ActiveXControl;

            // Imposta i dati del controllo includendo il CLSID copiandoli in un array esistente
            Array.Copy(dummyClsid, unknownControl.Data, dummyClsid.Length);

            // Leggi e visualizza le informazioni della proprietà Data
            Console.WriteLine($"Unknown control data length: {unknownControl.Data.Length}");
            Console.WriteLine($"Control type: {unknownControl.Type}");

            // Dimostrare la persistenza dei dati di controllo nel file di output
            workbook.Save("UnknownControlDataDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


