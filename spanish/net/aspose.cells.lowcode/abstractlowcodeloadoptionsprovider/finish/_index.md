---
title: "AbstractLowCodeLoadOptionsProvider.Finish"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AbstractLowCodeLoadOptionsProvider. Libera recursos después de procesar la parte actual de la entrada"
type: docs
url: /es/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/finish/
---
## AbstractLowCodeLoadOptionsProvider.Finish method

Libera recursos después de procesar la parte actual de la entrada.

```csharp
public virtual void Finish(LowCodeLoadOptions part)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| parte | LowCodeLoadOptions | las opciones de carga usadas para la parte dividida actualmente. |

### Observaciones

Por defecto, este método simplemente cierra el stream especificado por el [`InputStream`](../../lowcodeloadoptions/inputstream/) directamente (si las opciones de carga especificaron un Stream como origen). El usuario puede sobrescribir este método para controlar cómo liberar recursos según sus requisitos y la implementación de [`Current`](../current/).

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.Collections;

    public class AbstractLowCodeLoadOptionsProviderMethodFinishWithLowCodeLoadOptionsDemo
    {
        public static void Run()
        {
            string[] files = { "file1.xlsx", "file2.xlsx", "file3.xlsx" };

            CustomLoadOptionsProvider provider = new CustomLoadOptionsProvider(files);

            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.OutputFile = "result.xlsx";
            saveOptions.SaveFormat = SaveFormat.Xlsx;

            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            mergeOptions.LoadOptionsProvider = provider;
            mergeOptions.SaveOptions = saveOptions;

            SpreadsheetMerger.Process(mergeOptions);
        }
    }

    public class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
    {       

        public IEnumerator fileIter;
        public CustomLoadOptionsProvider(string[] files)
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


