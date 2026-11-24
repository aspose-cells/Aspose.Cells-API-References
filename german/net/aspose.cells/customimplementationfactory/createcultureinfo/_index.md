---
title: "CustomImplementationFactory.CreateCultureInfo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomImplementationFactory-Methode. Erstellt ein CultureInfo-Objekt anhand einer angegebenen ID"
type: docs
url: /de/net/aspose.cells/customimplementationfactory/createcultureinfo/
---
## CustomImplementationFactory.CreateCultureInfo method

Erstelle ein CultureInfo-Objekt anhand der angegebenen ID.

```csharp
public virtual CultureInfo CreateCultureInfo(int lcid)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| LCID | Int32 |  |

### Rückgabewert

Die CultureInfo-Instanz.

### Hinweise

Diese Implementierung ist für folgende Situationen nützlich: 1. Einige Kulturen werden möglicherweise nicht von der Umgebung des Benutzers unterstützt und das Erstellen des erforderlichen CultureInfo mit dem angegebenen Bezeichner kann eine Ausnahme auslösen. Um die Ausnahme zu vermeiden, kann der Benutzer diese Methode überschreiben, um eine gültige CultureInfo‑Instanz für die nicht unterstützte Kultur bereitzustellen. 2. Der Benutzer möchte möglicherweise einige benutzerdefinierte Eigenschaften für bestimmte Kulturen festlegen, um das erwartete Formatierungsergebnis zu erhalten. Zu diesem Zweck kann der Benutzer diese Methode überschreiben, um die CultureInfo‑Instanz mit den vom Benutzer angegebenen Eigenschaften zu liefern. Bitte beachten Sie, dass die Eigenschaft UseUserOverride der zurückgegebenen CultureInfo‑Instanz das formatierte Ergebnis beeinflussen kann. Ist sie false, können einige Eigenschaften der zurückgegebenen CultureInfo‑Instanz von unserer integrierten Formatierungs‑Engine überschrieben werden, je nach den Formatierungsanforderungen verschiedener Szenarien. Ist sie true, ändern wir keine Eigenschaften und verwenden sie direkt zur Formatierung von Werten. Daher sollte der Benutzer, der benutzerdefinierte Eigenschaften für die zurückgegebene CultureInfo‑Instanz festgelegt hat, sicherstellen, dass UseUserOverride true ist.

### Beispiele

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
                // Erstellen Sie eine Instanz von CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Rufe CreateCultureInfo mit einer gültigen LCID (1033 für Englisch – Vereinigte Staaten) auf
                int lcid = 1033;
                CultureInfo cultureInfo = factory.CreateCultureInfo(lcid);

                // Ergebnisse anzeigen
                Console.WriteLine($"CultureInfo created successfully with LCID: {lcid}");
                Console.WriteLine($"Culture Name: {cultureInfo.Name}");
                Console.WriteLine($"Display Name: {cultureInfo.DisplayName}");
                Console.WriteLine($"English Name: {cultureInfo.EnglishName}");

                // Demonstriere das Setzen der Fabrik in CellsHelper
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

### Siehe auch

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


