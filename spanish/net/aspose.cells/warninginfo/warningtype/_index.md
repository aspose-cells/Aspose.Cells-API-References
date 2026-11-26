---
title: "WarningInfo.WarningType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WarningInfo. Obtenga el tipo de advertencia"
type: docs
url: /es/net/aspose.cells/warninginfo/warningtype/
---
## WarningInfo.WarningType property

Obtener tipo de advertencia.

```csharp
[Obsolete("Use WarningInfo.Type property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public WarningType WarningType { get; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad WarningInfo.Type. Esta propiedad será eliminada 12 meses después, a partir de diciembre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyWarningTypeDemo
    {
        public static void Run()
        {
            // Cree un libro de trabajo y genere una advertencia
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Esto generará una advertencia al guardar con funciones no compatibles
            workbook.Settings.WarningCallback = new WarningCallback();
            
            // Guardar con un formato que pueda causar advertencias
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }

    internal class WarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            // Demostrar el uso de la propiedad WarningType
            Console.WriteLine("Warning: " + warningInfo.WarningType + " - " + warningInfo.Description);
            
            // Manejar tipos de advertencia específicos
            if (warningInfo.WarningType == WarningType.UnsupportedFileFormat)
            {
                Console.WriteLine("Unsupported format warning detected!");
            }
        }
    }
}
```

### Ver también

* enum [WarningType](../../warningtype/)
* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


