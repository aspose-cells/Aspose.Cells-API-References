---
title: "Clase AbstractInterruptMonitor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.AbstractInterruptMonitor. Monitor de solicitudes de interrupción en todas las operaciones que consumen tiempo"
type: docs
url: /es/net/aspose.cells/abstractinterruptmonitor/
---
## AbstractInterruptMonitor class

Monitorea las solicitudes de interrupción en todas las operaciones que consumen mucho tiempo.

```csharp
public abstract class AbstractInterruptMonitor
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| abstract [IsInterruptionRequested](../../aspose.cells/abstractinterruptmonitor/isinterruptionrequested/) { get; } | Indica si se solicita una interrupción para la operación actual. Si es true, la operación actual será interrumpida. La implementación debe realizar una verificación rápida y eficiente aquí, de lo contrario podría convertirse en otro cuello de botella para el procedimiento. |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception/) { get; } | Cuando el procedimiento se interrumpe, si se debe terminar el procedimiento silenciosamente o lanzar una Excepción. El valor predeterminado es false, es decir, cuando [`IsInterruptionRequested`](./isinterruptionrequested/) es true, se lanzará una [`CellsException`](../cellsexception/) con el código Interrupted. |

### Ejemplos

```csharp
using Aspose.Cells;
using System;
using System.Reflection.Metadata.Ecma335;

namespace AsposeCellsExamples
{
    // Implementación personalizada de AbstractInterruptMonitor
    public class CustomInterruptMonitor : AbstractInterruptMonitor
    {
        //el archivo de resultados es correcto
        public override bool IsInterruptionRequested
        {
            get
            {
                Console.WriteLine("Get the return value of whether to interrupt the program===");
                // Lógica para determinar si se solicita interrupción
                return false; // Change this based on your logic
            }
        }

        public override bool TerminateWithoutException
        {
            get => false; // Change this based on your logic
        }

        //// el archivo de resultados se bloquea
        //public override bool IsInterruptionRequested
        //{
        //    get
        //    {
        //        Console.WriteLine("Obtener el valor de retorno de si interrumpir el programa===");
        //        // Lógica para determinar si se solicita interrupción
        //        //return false; // Cambia esto según tu lógica
        //        return true;
        //    }
        //}

        //public override bool TerminateWithoutException
        //{
        //    get => true; // Cambia esto según tu lógica
        //}
    }

    public class InterruptMonitorDemo
    {
        public static void RunDemo()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].Formula = "=A1+A2";

            // Crear una instancia de CustomInterruptMonitor
            CustomInterruptMonitor monitor = new CustomInterruptMonitor();

            // Establecer opciones de carga con el monitor de interrupción personalizado
            LoadOptions loadOptions = new LoadOptions
            {
                InterruptMonitor = monitor
            };

            // Cargar el libro de trabajo con las opciones especificadas
            workbook = new Workbook("Sample.xlsx", loadOptions);

            // Realizar cálculos
            workbook.CalculateFormula();

            // Guarda el libro de trabajo
            workbook.Save("InterruptMonitorDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


