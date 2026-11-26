---
title: "LowCodeMergeOptions.LoadOptionsProvider"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de LowCodeMergeOptions. Proveedor de opciones de guardado para guardar las partes divididas"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodemergeoptions/loadoptionsprovider/
---
## LowCodeMergeOptions.LoadOptionsProvider property

Proveedor de opciones de guardado para guardar las partes divididas.

```csharp
public AbstractLowCodeLoadOptionsProvider LoadOptionsProvider { get; set; }
```

### Observaciones

Si se especifica esta propiedad, [`LoadOptions`](../../../aspose.cells/loadoptions/) no tiene efecto porque la salida de cada parte dividida será especificada por el proveedor.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeMergeOptionsPropertyLoadOptionsProviderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una instancia de LowCodeMergeOptions
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();

            // Mostrar el valor actual de LoadOptionsProvider (debería ser null inicialmente)
            Console.WriteLine("Current LoadOptionsProvider value: " + (mergeOptions.LoadOptionsProvider == null ? "null" : "not null"));

            // Crear una implementación personalizada de LoadOptionsProvider
            mergeOptions.LoadOptionsProvider = new CustomLoadOptionsProvider();

            // Demostrar la configuración de la propiedad
            Console.WriteLine("After setting LoadOptionsProvider: " + (mergeOptions.LoadOptionsProvider == null ? "null" : "not null"));

            // Usar las opciones de fusión con el proveedor
            // Esto normalmente se usaría con métodos que procesan varios archivos
            // Para la demostración, solo verificaremos si el proveedor puede pasar al siguiente
            bool hasNext = mergeOptions.LoadOptionsProvider.MoveNext();
            Console.WriteLine("LoadOptionsProvider MoveNext result: " + hasNext);

            // Guarda el libro de trabajo
            workbook.Save("PropertyLoadOptionsProviderDemo.xlsx");
        }

        private class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
        {
            private int counter = 0;
            private readonly LowCodeLoadOptions options = new LowCodeLoadOptions();

            public override LowCodeLoadOptions Current => options;

            public override bool MoveNext()
            {
                // Simular tener 3 archivos para procesar
                if (counter < 3)
                {
                    counter++;
                    return true;
                }
                return false;
            }

            public override void Finish(LowCodeLoadOptions part)
            {
                // La lógica de limpieza o finalización iría aquí
            }
        }
    }
}
```

### Ver también

* class [AbstractLowCodeLoadOptionsProvider](../../abstractlowcodeloadoptionsprovider/)
* class [LowCodeMergeOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


