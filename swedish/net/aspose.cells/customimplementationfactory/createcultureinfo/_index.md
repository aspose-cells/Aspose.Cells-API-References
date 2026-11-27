---
title: "CustomImplementationFactory.CreateCultureInfo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomImplementationFactory‑metod. Skapa en CultureInfo med angivet id"
type: docs
url: /sv/net/aspose.cells/customimplementationfactory/createcultureinfo/
---
## CustomImplementationFactory.CreateCultureInfo method

Skapa en CultureInfo med givet id.

```csharp
public virtual CultureInfo CreateCultureInfo(int lcid)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| lcid | Int32 |  |

### Returvärde

CultureInfo‑instansen.

### Anmärkningar

Denna implementation är användbar i följande situationer: 1. Vissa kulturer kanske inte stöds av användarens miljö och att skapa den erforderliga CultureInfo med angivet identifierare kan orsaka ett undantag. För att undvika undantaget kan användaren åsidosätta denna metod för att tillhandahålla en giltig CultureInfo‑instans för den icke‑stödda kulturen. 2. Användaren kan vilja ange vissa anpassade egenskaper för vissa kulturer för att få förväntat formatresultat. För detta ändamål kan användaren åsidosätta metoden för att tillhandahålla CultureInfo‑instansen med de av användaren specificerade egenskaperna. Observera att egenskapen UseUserOverride för den returnerade CultureInfo‑instansen kan påverka det formaterade resultatet. Om den är falsk kan vissa egenskaper i den returnerade CultureInfo‑instansen åsidosättas av vår inbyggda formateringsmotor enligt formateringskraven i olika scenarier. Om den är sann kommer vi inte att ändra några egenskaper och använda den för att formatera värden direkt. Så, om användaren har specificerat anpassade egenskaper för den returnerade CultureInfo‑instansen, se till att dess UseUserOverride är sann.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Globalization;

    public class CustomImplementationFactoryMethodCreateCultureInfoWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                // Skapa en instans av CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Anropa CreateCultureInfo med ett giltigt LCID (1033 för engelska – USA)
                int lcid = 1033;
                CultureInfo cultureInfo = factory.CreateCultureInfo(lcid);

                // Visa resultaten
                Console.WriteLine($"CultureInfo created successfully with LCID: {lcid}");
                Console.WriteLine($"Culture Name: {cultureInfo.Name}");
                Console.WriteLine($"Display Name: {cultureInfo.DisplayName}");
                Console.WriteLine($"English Name: {cultureInfo.EnglishName}");

                // Demonstrera att sätta fabriken i CellsHelper
                CellsHelper.CustomImplementationFactory = factory;
                Console.WriteLine("CustomImplementationFactory set in CellsHelper.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling CreateCultureInfo: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


