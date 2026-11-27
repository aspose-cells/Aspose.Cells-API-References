---
title: "Workbook.Copy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook method. Kopierar ett annat Workbook-objekt"
type: docs
url: /sv/net/aspose.cells/workbook/copy/
---
## Copy(Workbook, CopyOptions) {#copy_1}

Kopierar ett annat Workbook-objekt.

```csharp
public void Copy(Workbook source, CopyOptions copyOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| källa | Arbetsbok | Käll Workbook-objekt. |
| copyOptions | CopyOptions | Alternativen för att kopiera en annan workbook. |

### Anmärkningar

Det är mycket enkelt att klona en Excel-fil.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyWithWorkbookCopyOptionsDemo
    {
        public static void Run()
        {
            // Källworkbook med makron
            Workbook sourceWorkbook = new Workbook("source_with_macros.xlsm");
            
            // Destination workbook (tom eller befintlig)
            Workbook destWorkbook = new Workbook();
            
            // Konfigurera kopieringsalternativ för att behålla makron
            CopyOptions options = new CopyOptions();
            options.KeepMacros = true;
            
            // Kopiera innehåll från källworkbook till destinationsworkbook
            sourceWorkbook.Copy(destWorkbook, options);
            
            // Spara resultatet
            destWorkbook.Save("output_with_macros.xlsm");
        }
    }
}
```

### Se även

* class [CopyOptions](../../copyoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Workbook) {#copy}

Kopierar data från ett käll-Workbook-objekt.

```csharp
public void Copy(Workbook source)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| källa | Arbetsbok | Käll Workbook-objekt. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyWithWorkbookDemo
    {
        public static void Run()
        {
            // Käll- och utdatafilvägar
            string sourceFile = "source.xlsx";
            string outputFile = "output.xlsx";

            // Läs in källarbetsboken
            Workbook sourceWorkbook = new Workbook(sourceFile);

            // Skapa en ny workbook och kopiera innehåll från källworkbook
            Workbook destinationWorkbook = new Workbook();
            destinationWorkbook.Copy(sourceWorkbook);

            // Spara den kopierade workbooken
            destinationWorkbook.Save(outputFile);
            
            Console.WriteLine("Workbook copied successfully.");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


