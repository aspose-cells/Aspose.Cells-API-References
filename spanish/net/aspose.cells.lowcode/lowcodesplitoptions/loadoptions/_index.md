---
title: "LowCodeSplitOptions.LoadOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodeSplitOptions. Opciones de carga para cargar la hoja de cálculo que se dividirá"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesplitoptions/loadoptions/
---
## LowCodeSplitOptions.LoadOptions property

Opciones de carga para cargar la hoja de cálculo que se dividirá.

```csharp
public LowCodeLoadOptions LoadOptions { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertyLoadOptionsDemo
    {
        public static void Run()
        {
            // Crear una instancia de opciones de división
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();

            // Inicializar opciones de carga
            splitOptions.LoadOptions = new LowCodeLoadOptions();

            // Crear nuevas opciones de carga con diferentes configuraciones (usando propiedades disponibles)
            splitOptions.LoadOptions = new LowCodeLoadOptions();
            
            // Demostrar la configuración final
            Console.WriteLine("LoadOptions configured with InputFile: " + splitOptions.LoadOptions.InputFile);
        }
    }
}
```

### Ver también

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


