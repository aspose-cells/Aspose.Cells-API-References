---
title: "CellsHelper.CreateSafeSheetName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-metod. Kontrollerar det angivna bladnamnet och skapar ett giltigt när det behövs. Om det angivna bladnamnet följer Excels regler för bladnamn returneras det. Annars kommer strängen att trunkeras om längden överskrider gränsen och ogiltiga tecken kommer att ersättas med   och sedan returneras det ombyggda strängvärdet."
type: docs
url: /sv/net/aspose.cells/cellshelper/createsafesheetname/
---
## CreateSafeSheetName(string) {#createsafesheetname}

Kontrollerar angivet bladnamn och skapar ett giltigt när det behövs. Om det angivna bladnamnet följer Excels regler för bladnamn returneras det. Annars kommer strängen att trunkeras om längden överskrider gränsen och ogiltiga tecken ersätts med ' ', sedan returneras det återuppbyggda strängvärdet.

```csharp
public static string CreateSafeSheetName(string nameProposal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nameProposal | String | bladnamn att använda |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCreateSafeSheetNameWithStringDemo
    {
        public static void Run()
        {
            string unsafeName = "sheet*/test*/?#";
            string safeName = CellsHelper.CreateSafeSheetName(unsafeName);
            Console.WriteLine("Original name: " + unsafeName);
            Console.WriteLine("Safe name: " + safeName);
        }
    }
}
```

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateSafeSheetName(string, char) {#createsafesheetname_1}

Kontrollerar angivet bladnamn och skapar ett giltigt när det behövs. Om det angivna bladnamnet följer Excels regler för bladnamn returneras det. Annars kommer strängen att trunkeras om längden överskrider gränsen och ogiltiga tecken ersätts med det angivna tecknet, sedan returneras det återuppbyggda strängvärdet.

```csharp
public static string CreateSafeSheetName(string nameProposal, char replaceChar)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nameProposal | String | bladnamn att använda |
| replaceChar | Char | tecken som kommer att användas för att ersätta ogiltiga tecken i det angivna bladnamnet |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCreateSafeSheetNameWithStringCharDemo
    {
        public static void Run()
        {
            // Exempel 1: Skapa säkert bladnamn med standardersättningstecken
            string name1 = CellsHelper.CreateSafeSheetName("sheet*/test*/?#");
            Console.WriteLine("Safe sheet name (default replacement): " + name1);

            // Exempel 2: Skapa säkert bladnamn med anpassat ersättningstecken 'A'
            string name2 = CellsHelper.CreateSafeSheetName("sheet*/test*/?#", 'A');
            Console.WriteLine("Safe sheet name (custom replacement): " + name2);
        }
    }
}
```

### Se även

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


