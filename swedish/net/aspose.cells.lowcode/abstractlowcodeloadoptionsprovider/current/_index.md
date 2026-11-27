---
title: "AbstractLowCodeLoadOptionsProvider.Current"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractLowCodeLoadOptionsProvider-egenskap. Hämtar laddningsalternativen från vilka data för den för närvarande bearbetade delen ska läsas"
type: docs
url: /sv/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/current/
---
## AbstractLowCodeLoadOptionsProvider.Current property

Hämtar inläsningsalternativen från vilka data för den för närvarande bearbetade delen ska läsas in.

```csharp
public abstract LowCodeLoadOptions Current { get; }
```

### Exempel

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
            // Initiera anpassad leverantör med våra laddningsalternativ
            CustomProvider provider = new CustomProvider(files);
            
            int counter = 1;
            while (provider.MoveNext())
            {
                // Få åtkomst till Current-egenskapen för att hämta aktiva laddningsalternativ
                Console.WriteLine($"Processing set {counter}");
                    
                // Skapa arbetsbok med den aktuella laddningsalternativens inmatningsfil/ström
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

                // Demonstrera påverkan av alternativet som har tagits bort på grund av saknad egenskap
                worksheet.Cells["A1"].Value = "Sample Value";

                // Spara resultatet
                workbook.Save($"CurrentDemo_{counter}.xlsx");
                counter++;
            }
        }
    }

    // Anpassad leverantörsimplementation med IDisposable
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

### Se även

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [AbstractLowCodeLoadOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


