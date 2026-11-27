---
title: "LowCodeMergeOptions.LoadOptionsProvider"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeMergeOptions-egenskap. Leverantör av sparaalternativ för att spara de delade delarna"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodemergeoptions/loadoptionsprovider/
---
## LowCodeMergeOptions.LoadOptionsProvider property

Leverantör av sparaalternativ för att spara de delade delarna.

```csharp
public AbstractLowCodeLoadOptionsProvider LoadOptionsProvider { get; set; }
```

### Anmärkningar

Om denna egenskap anges, [`LoadOptions`](../../../aspose.cells/loadoptions/) har ingen effekt eftersom utdata för varje delad del kommer att specificeras av leverantören.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeMergeOptionsPropertyLoadOptionsProviderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av LowCodeMergeOptions
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();

            // Visa det aktuella värdet för LoadOptionsProvider (ska vara null initialt)
            Console.WriteLine("Current LoadOptionsProvider value: " + (mergeOptions.LoadOptionsProvider == null ? "null" : "not null"));

            // Skapa en anpassad LoadOptionsProvider-implementation
            mergeOptions.LoadOptionsProvider = new CustomLoadOptionsProvider();

            // Visa hur egenskapen sätts
            Console.WriteLine("After setting LoadOptionsProvider: " + (mergeOptions.LoadOptionsProvider == null ? "null" : "not null"));

            // Använd sammanslagningsalternativen med leverantören
            // Detta skulle vanligtvis användas med metoder som bearbetar flera filer
            // För demonstration kommer vi bara att kontrollera om leverantören kan gå till nästa
            bool hasNext = mergeOptions.LoadOptionsProvider.MoveNext();
            Console.WriteLine("LoadOptionsProvider MoveNext result: " + hasNext);

            // Spara arbetsboken
            workbook.Save("PropertyLoadOptionsProviderDemo.xlsx");
        }

        private class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
        {
            private int counter = 0;
            private readonly LowCodeLoadOptions options = new LowCodeLoadOptions();

            public override LowCodeLoadOptions Current => options;

            public override bool MoveNext()
            {
                // Simulera att ha 3 filer att bearbeta
                if (counter < 3)
                {
                    counter++;
                    return true;
                }
                return false;
            }

            public override void Finish(LowCodeLoadOptions part)
            {
                // Rensnings- eller avslutningslogik skulle placeras här
            }
        }
    }
}
```

### Se även

* class [AbstractLowCodeLoadOptionsProvider](../../abstractlowcodeloadoptionsprovider/)
* class [LowCodeMergeOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


