---
title: "Interfaz IWarningCallback"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Interfaz Aspose.Cells.IWarningCallback. Interfaz de devolución de llamada de advertencia"
type: docs
url: /es/net/aspose.cells/iwarningcallback/
---
## IWarningCallback interface

Interfaz de devolución de llamada de advertencia.

```csharp
public interface IWarningCallback
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Warning](../../aspose.cells/iwarningcallback/warning/)(WarningInfo) | Nuestro callback solo necesita implementar el método "Warning". |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IWarningCallbackDemo : IWarningCallback
    {
        // Implementando el método Warning de la interfaz IWarningCallback
        public void Warning(WarningInfo warningInfo)
        {
            // Mostrar el mensaje de advertencia
            Console.WriteLine("Warning: " + warningInfo.WarningType + " - " + warningInfo.Description);
        }

        public static void IWarningCallbackExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Establecer la devolución de llamada de advertencia
            workbook.Settings.WarningCallback = new IWarningCallbackDemo();

            // Cargar un libro de trabajo con posibles advertencias
            try
            {
                workbook = new Workbook("example.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception: " + ex.Message);
            }

            // Guarda el libro de trabajo
            workbook.Save("IWarningCallbackExample.xlsx");
        }
    }

}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


