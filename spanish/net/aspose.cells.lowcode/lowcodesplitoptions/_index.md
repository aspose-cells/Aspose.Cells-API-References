---
title: "Clase LowCodeSplitOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.LowCode.LowCodeSplitOptions. Opciones para dividir la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesplitoptions/
---
## LowCodeSplitOptions class

Opciones para dividir la hoja de cálculo.

```csharp
public class LowCodeSplitOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [LowCodeSplitOptions](lowcodesplitoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [LoadOptions](../../aspose.cells.lowcode/lowcodesplitoptions/loadoptions/) { get; set; } | Opciones de carga para cargar la hoja de cálculo que se dividirá. |
| [SaveOptions](../../aspose.cells.lowcode/lowcodesplitoptions/saveoptions/) { get; set; } | Opciones de guardado para guardar las partes divididas. |
| [SaveOptionsProvider](../../aspose.cells.lowcode/lowcodesplitoptions/saveoptionsprovider/) { get; set; } | Proveedor de opciones de guardado para guardar las partes divididas. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeSplitOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Poblar la hoja de cálculo con datos de ejemplo
            worksheet.Cells["A1"].PutValue("Sample Data for Splitting");
            
            // Crea una instancia de LowCodeSplitOptions
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            
            // Configura LoadOptions (ejemplo: maneja una fuente protegida con contraseña)
            splitOptions.LoadOptions = new LowCodeLoadOptions();
            
            // Configura SaveOptions (ejemplo: establece el formato de salida predeterminado)
            splitOptions.SaveOptions = new LowCodeSaveOptions();
            
            // Implementa un proveedor personalizado de SaveOptions para configuraciones de salida dinámicas
            splitOptions.SaveOptionsProvider = new CustomSaveOptionsProvider();
            
            // Ejemplo de integración: Divide el libro de trabajo en partes usando las opciones configuradas
            // (Supón la existencia de un método como LowCodeEngine.Split(workbook, splitOptions, "outputDir"))
            // LowCodeEngine.Split(workbook, splitOptions, "OutputDirectory");
            
            // Guarda el libro de trabajo original para la demostración
            workbook.Save("LowCodeSplitOptionsDemo.xlsx");
        }

        // Implementación personalizada de SaveOptionsProvider
        private class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
        {
            public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
            {
                // Lógica de ejemplo: Alternar configuraciones según el índice de división
                return new LowCodeSaveOptions();
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


