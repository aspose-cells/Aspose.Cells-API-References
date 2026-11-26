---
title: "AbstractLowCodeSaveOptionsProvider.Finish"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AbstractLowCodeSaveOptionsProvider. Libera recursos después de procesar la parte dividida actualmente"
type: docs
url: /es/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/
---
## AbstractLowCodeSaveOptionsProvider.Finish method

Libera recursos después de procesar la parte dividida actual.

```csharp
public virtual void Finish(LowCodeSaveOptions part)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| parte | LowCodeSaveOptions | las opciones de guardado usadas para la parte actualmente dividida. |

### Observaciones

Por defecto, este método solo cierra el flujo especificado por el [`OutputStream`](../../lowcodesaveoptions/outputstream/) directamente (si las opciones de guardado especificaron un Stream como destino). El usuario puede sobrescribir este método para controlar cómo liberar recursos según sus requisitos y la implementación de [`GetSaveOptions`](../getsaveoptions/).

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeSaveOptionsProviderMethodFinishWithLowCodeSaveOptionsDemo
    {
        public static void Run()
        {

            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "split.xlsx";

            // Crea una instancia concreta del proveedor
            var provider = new CustomLowCodeSaveOptionsProvider();

            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            splitOptions.SaveOptionsProvider = provider;
            splitOptions.LoadOptions = loadOptions;

            SpreadsheetSplitter.Process(splitOptions);
                     
          
        }
    }

    // Implementación concreta de AbstractLowCodeSaveOptionsProvider
    public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override void Finish(LowCodeSaveOptions part)
        { 
            base.Finish(part);
        }
        // Implementa el método abstracto requerido
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            LowCodeSaveOptions result = new LowCodeSaveOptions();
            result.SaveFormat = SaveFormat.Xlsx;
            result.OutputFile = partInfo.SheetName + "_split.xlsx";
            Console.WriteLine(result.OutputFile);
            return result;
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


