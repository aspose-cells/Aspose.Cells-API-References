---
title: "Cells.MultiThreadReading"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Obtiene o establece si el modelo de datos de celdas debe admitir la lectura MultiThread. El valor predeterminado de esta propiedad es false"
type: docs
url: /es/net/aspose.cells/cells/multithreadreading/
---
## Cells.MultiThreadReading property

Obtiene o establece si el modelo de datos de las celdas debe soportar lectura Multi-Thread. El valor predeterminado de esta propiedad es false.

```csharp
public bool MultiThreadReading { get; set; }
```

### Observaciones

Si hay varios hilos leyendo objetos Row/Cell en esta colección de forma concurrente, esta propiedad debe establecerse en true; de lo contrario, pueden producirse resultados inesperados. Admitir la lectura Multi-Thread puede degradar el rendimiento al acceder a objetos Row/Cell de esta colección. Tenga en cuenta que algunas funciones no pueden admitir la lectura Multi-Thread, como el formato de valores (por [`StringValue`](../../cell/stringvalue/), [`DisplayStringValue`](../../cell/displaystringvalue/), etc.). Por lo tanto, incluso con esta propiedad establecida en true, esas API aún pueden dar resultados inesperados al leer con Multi-Thread.

### Ejemplos

```csharp
using System;
using System.Threading;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMultiThreadReadingDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Habilitar la lectura multi-thread
            cells.MultiThreadReading = true;

            // Configurar estilo para la primera columna
            Style style = wb.CreateStyle();
            style.Custom = "yyyy-mm-dd";
            StyleFlag sf = new StyleFlag();
            sf.All = true;
            cells.Columns[0].ApplyStyle(style, sf);

            // Rellenar celdas con datos de ejemplo
            int rowCount = 1000;
            for (int i = 0; i < rowCount; i++)
            {
                cells[i, 0].PutValue(DateTime.Now.AddDays(i).ToOADate());
            }

            // Crear hilos para leer valores de celdas
            int threadCount = 5;
            int cellsPerThread = rowCount / threadCount;
            int[] finishedCount = new int[1];
            System.Text.StringBuilder errors = new System.Text.StringBuilder();

            for (int i = 0; i < threadCount; i++)
            {
                int start = i * cellsPerThread;
                int end = (i == threadCount - 1) ? rowCount : start + cellsPerThread;
                
                Thread t = new Thread(() => 
                {
                    try
                    {
                        for (int row = start; row < end; row++)
                        {
                            object value = cells[row, 0].Value;
                            Console.WriteLine($"Thread {Thread.CurrentThread.ManagedThreadId}: Cell[{row},0] = {value}");
                        }
                        Interlocked.Increment(ref finishedCount[0]);
                    }
                    catch (Exception ex)
                    {
                        lock (errors)
                        {
                            errors.AppendLine($"Thread {Thread.CurrentThread.ManagedThreadId} error: {ex.Message}");
                        }
                    }
                });
                t.Start();
            }

            // Esperar a que todos los hilos terminen
            while (finishedCount[0] < threadCount)
            {
                Thread.Sleep(200);
            }

            if (errors.Length > 0)
            {
                Console.WriteLine("Errors occurred:");
                Console.WriteLine(errors.ToString());
            }
            else
            {
                Console.WriteLine("All threads completed successfully");
            }
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


