---
title: "Clase LowCodeMergeOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.LowCode.LowCodeMergeOptions. Opciones para combinar varios archivos de plantilla en uno"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodemergeoptions/
---
## LowCodeMergeOptions class

Opciones para combinar múltiples archivos de plantilla en uno.

```csharp
public class LowCodeMergeOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [LowCodeMergeOptions](lowcodemergeoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [LoadOptionsProvider](../../aspose.cells.lowcode/lowcodemergeoptions/loadoptionsprovider/) { get; set; } | Proveedor de opciones de guardado para guardar las partes divididas. |
| [SaveOptions](../../aspose.cells.lowcode/lowcodemergeoptions/saveoptions/) { get; set; } | Opciones de guardado para guardar las partes divididas. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeMergeOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Crear y configurar LowCodeMergeOptions
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            
            // Establecer opciones de guardado para el formato de salida
            mergeOptions.SaveOptions = new LowCodeSaveOptions();
            
            // Asignar proveedor de opciones de carga personalizado
            mergeOptions.LoadOptionsProvider = new CustomLoadOptionsProvider();
            
            // Ejemplo de integración (uso hipotético con funcionalidad de combinación)
            // Esto normalmente se llamaría con rutas de archivo reales
            // Workbook.Merge(new string[] { "template1.xlsx", "template2.xlsx" }, mergeOptions);
            
            // Guardar el libro de trabajo (con fines de demostración)
            workbook.Save("LowCodeMergeOptionsDemo.xlsx");
        }
    }

    // Proveedor personalizado que implementa la clase abstracta
    public class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
    {
        public override bool MoveNext()
        {
            // Implementación mínima para cumplir con el requisito abstracto
            return false;
        }

        public override LowCodeLoadOptions Current
        {
            get { throw new InvalidOperationException(); }
        }

        public LoadOptions GetLoadOptions(string fileName)
        {
            if (fileName.EndsWith(".xlsx", StringComparison.OrdinalIgnoreCase))
            {
                return new LoadOptions(LoadFormat.Xlsx);
            }
            return new LoadOptions();
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


