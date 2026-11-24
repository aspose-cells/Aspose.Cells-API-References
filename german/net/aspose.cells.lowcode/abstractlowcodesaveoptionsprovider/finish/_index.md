---
title: "AbstractLowCodeSaveOptionsProvider.Finish"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractLowCodeSaveOptionsProvider-Methode. Gibt Ressourcen frei, nachdem der aktuell aufgeteilte Teil verarbeitet wurde"
type: docs
url: /de/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/
---
## AbstractLowCodeSaveOptionsProvider.Finish method

Gibt Ressourcen frei, nachdem der aktuell geteilte Teil verarbeitet wurde.

```csharp
public virtual void Finish(LowCodeSaveOptions part)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Teil | LowCodeSaveOptions | die Speicheroptionen, die für den aktuell aufgeteilten Teil verwendet werden. |

### Hinweise

Standardmäßig schließt diese Methode einfach den durch [`OutputStream`](../../lowcodesaveoptions/outputstream/) angegebenen Stream direkt (wenn die Speicheroptionen einen Stream als Ziel angegeben haben). Der Benutzer kann diese Methode überschreiben, um zu steuern, wie Ressourcen gemäß seinen Anforderungen und der Implementierung von [`GetSaveOptions`](../getsaveoptions/) freigegeben werden.

### Beispiele

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

            // Erstelle eine konkrete Provider-Instanz
            var provider = new CustomLowCodeSaveOptionsProvider();

            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            splitOptions.SaveOptionsProvider = provider;
            splitOptions.LoadOptions = loadOptions;

            SpreadsheetSplitter.Process(splitOptions);
                     
          
        }
    }

    // Konkrete Implementierung von AbstractLowCodeSaveOptionsProvider
    public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override void Finish(LowCodeSaveOptions part)
        { 
            base.Finish(part);
        }
        // Implementiere die erforderliche abstrakte Methode
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

### Siehe auch

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


