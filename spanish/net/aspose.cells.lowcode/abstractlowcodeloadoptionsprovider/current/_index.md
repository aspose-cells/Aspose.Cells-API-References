---
title: "AbstractLowCodeLoadOptionsProvider.Current"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AbstractLowCodeLoadOptionsProvider. Obtiene las opciones de carga desde las cuales cargar datos de la parte procesada actualmente"
type: docs
url: /es/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/current/
---
## AbstractLowCodeLoadOptionsProvider.Current property

Obtiene las opciones de carga desde las cuales cargar los datos de la parte procesada actualmente.

```csharp
public abstract LowCodeLoadOptions Current { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.Collections;

    public class AbstractLowCodeLoadOptionsProviderPropertyCurrentDemo
    {
        public static void Run()
        {
            string[] files = { "file1.xlsx", "file2.xlsx", "file3.xlsx" };
            // Inicializar proveedor personalizado con nuestras opciones de carga
            CustomProvider provider = new CustomProvider(files);
            
            int counter = 1;
            while (provider.MoveNext())
            {
                // Acceder a la propiedad Current para obtener las opciones de carga activas
                Console.WriteLine($"Processing set {counter}");
                    
                // Crear libro de trabajo usando el archivo/stream de entrada de las opciones de carga actuales
                Workbook workbook;
                if (provider.Current.InputFile != null)
                {
                    workbook = new Workbook(provider.Current.InputFile);
                }
                else if (provider.Current.InputStream != null)
                {
                    workbook = new Workbook(provider.Current.InputStream);
                }
                else
                {
                    workbook = new Workbook();
                }

                Worksheet worksheet = workbook.Worksheets[0];

                // Demostrar el impacto de la opción eliminado debido a la falta de la propiedad
                worksheet.Cells["A1"].Value = "Sample Value";

                // Guardar resultado
                workbook.Save($"CurrentDemo_{counter}.xlsx");
                counter++;
            }
        }
    }

    // Implementación de proveedor personalizado con IDisposable
    public class CustomProvider : AbstractLowCodeLoadOptionsProvider
    {
        
        public IEnumerator fileIter;

        public CustomProvider(string[] files)
        {
            fileIter = files.GetEnumerator();
            current = new LowCodeLoadOptions();
        }
        private LowCodeLoadOptions current;

        public override LowCodeLoadOptions Current => current;

        public override bool MoveNext()
        {
            if (fileIter.MoveNext())
            {
                current = new LowCodeLoadOptions();
                current.InputFile = fileIter.Current.ToString();
                return true;
            }

            return false;
        }

        public override void Finish(LowCodeLoadOptions part)
        {
            base.Finish(part);
        }

    }
}
```

### Ver también

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [AbstractLowCodeLoadOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


