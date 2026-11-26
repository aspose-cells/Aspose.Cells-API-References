---
title: "UnknownControl.Data"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad UnknownControl. Obtiene y establece los datos binarios del control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/unknowncontrol/data/
---
## UnknownControl.Data property

Obtiene y establece los datos binarios del control.

```csharp
public override byte[] Data { get; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un CLSID ficticio (identificador no válido)
            byte[] dummyClsid = new byte[16];

            // Agregar un control ActiveX desconocido usando ControlType.Unknown con todos los parámetros
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Unknown, 0, 0, 100, 100, 0, 0);

            // Acceder a la instancia UnknownControl
            UnknownControl unknownControl = (UnknownControl)shape.ActiveXControl;

            // Establecer los datos del control, incluido el CLSID, copiando en la matriz existente
            Array.Copy(dummyClsid, unknownControl.Data, dummyClsid.Length);

            // Leer y mostrar la información de la propiedad Data
            Console.WriteLine($"Unknown control data length: {unknownControl.Data.Length}");
            Console.WriteLine($"Control type: {unknownControl.Type}");

            // Demostrar la persistencia de los datos de control en el archivo de salida
            workbook.Save("UnknownControlDataDemo.xlsx");
        }
    }
}
```

### Ver también

* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


