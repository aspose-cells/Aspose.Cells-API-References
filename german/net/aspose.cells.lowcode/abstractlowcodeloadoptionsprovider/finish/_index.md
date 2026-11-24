---
title: "AbstractLowCodeLoadOptionsProvider.Finish"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractLowCodeLoadOptionsProvider-Methode. Gibt Ressourcen nach der Verarbeitung des aktuellen Eingabeteils frei"
type: docs
url: /de/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/finish/
---
## AbstractLowCodeLoadOptionsProvider.Finish method

Gibt Ressourcen nach der Verarbeitung des aktuellen Eingabeteils frei.

```csharp
public virtual void Finish(LowCodeLoadOptions part)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Teil | LowCodeLoadOptions | Die Ladeoptionen, die für den aktuell aufgeteilten Teil verwendet werden. |

### Hinweise

Standardmäßig schließt diese Methode einfach den durch [`InputStream`](../../lowcodeloadoptions/inputstream/) angegebenen Stream direkt (wenn die Ladeoptionen einen Stream als Quelle angegeben haben). Der Benutzer kann diese Methode überschreiben, um die Freigabe von Ressourcen gemäß seinen Anforderungen und der Implementierung von [`Current`](../current/) zu steuern.

### Beispiele

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

### Siehe auch

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [AbstractLowCodeLoadOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


