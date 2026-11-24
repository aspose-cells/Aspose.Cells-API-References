---
title: "AbstractLowCodeLoadOptionsProvider.Current"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractLowCodeLoadOptionsProvider-Eigenschaft. Gibt die Ladeoptionen zurück, aus denen die Daten des aktuell verarbeiteten Teils geladen werden"
type: docs
url: /de/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/current/
---
## AbstractLowCodeLoadOptionsProvider.Current property

Ermittelt die Ladeoptionen, aus denen die Daten des aktuell verarbeiteten Teils geladen werden.

```csharp
public abstract LowCodeLoadOptions Current { get; }
```

### Beispiele

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
            // Benutzerdefinierten Provider mit unseren Ladeoptionen initialisieren
            CustomProvider provider = new CustomProvider(files);
            
            int counter = 1;
            while (provider.MoveNext())
            {
                // Greifen Sie auf die Current-Eigenschaft zu, um die aktiven Ladeoptionen zu erhalten
                Console.WriteLine($"Processing set {counter}");
                    
                // Erstellen Sie eine Arbeitsmappe mit der Eingabedatei/-stream der aktuellen Ladeoptionen
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

                // Demonstriere die Auswirkung der Option, entfernt wegen fehlender Eigenschaft
                worksheet.Cells["A1"].Value = "Sample Value";

                // Ergebnis speichern
                workbook.Save($"CurrentDemo_{counter}.xlsx");
                counter++;
            }
        }
    }

    // Benutzerdefinierte Provider-Implementierung mit IDisposable
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

### Siehe auch

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [AbstractLowCodeLoadOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


