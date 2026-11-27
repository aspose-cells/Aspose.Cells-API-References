---
title: "License.SetLicense"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Licensmetod. Licenserar komponenten"
type: docs
url: /sv/net/aspose.cells.griddesktop/license/setlicense/
---
## SetLicense(Stream) {#setlicense}

Licensierar komponenten.

```csharp
public void SetLicense(Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | En ström som innehåller licensen. |

### Anmärkningar

Använd den här metoden för att läsa in en licens från en ström.

### Exempel

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)
```

### Se även

* class [License](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## SetLicense(string) {#setlicense_1}

Licensierar komponenten.

```csharp
public void SetLicense(string licenseName)
```

### Anmärkningar

Försöker hitta licensen på följande platser:

1. Explicit sökväg.

2. Mappen som innehåller Aspose-komponentens assembly.

3. Mappen som innehåller klientens anropande assembly.

4. Mappen som innehåller entry (startup)-assemblyn.

5. En inbäddad resurs i klientens anropande assembly.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Explicit sökväg.

2. En inbäddad resurs i klientens anropande assembly.

### Exempel

I det här exemplet kommer ett försök att hitta en licensfil med namnet MyLicense.lic att göras i mappen som innehåller komponenten, i mappen som innehåller den anropande samlingen, i mappen för startsamlingen och sedan i de inbäddade resurserna för den anropande samlingen.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As License = New License
license.SetLicense("MyLicense.lic")
```

Kan vara ett fullständigt eller kort filnamn eller namn på en inbäddad resurs. Använd en tom sträng för att växla till utvärderingsläge.

### Se även

* class [License](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


