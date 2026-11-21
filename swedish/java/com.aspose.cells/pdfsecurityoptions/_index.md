---
title: "PdfSecurityOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Alternativ för kryptering och åtkomstbehörigheter för ett PDF‑dokument."
type: docs
url: /sv/java/com.aspose.cells/pdfsecurityoptions/
---

**Inheritance:**
java.lang.Object
```
public class PdfSecurityOptions
```

Alternativ för kryptering och åtkomstbehörigheter för ett PDF‑dokument. PDF/A tillåter inte säkerhetsinställningar.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [PdfSecurityOptions()](#PdfSecurityOptions--) | Konstruktorn för PdfSecurityOptions |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAccessibilityExtractContent()](#getAccessibilityExtractContent--) | Anger om det ska tillåtas att extrahera text och grafik (för att stödja tillgänglighet för användare med funktionsnedsättningar eller för andra ändamål). |
| [getAnnotationsPermission()](#getAnnotationsPermission--) | Anger om det ska tillåtas att lägga till eller ändra textanteckningar, fylla i interaktiva formulärfält. |
| [getAssembleDocumentPermission()](#getAssembleDocumentPermission--) | Anger om det ska tillåtas att montera dokumentet (infoga, rotera eller ta bort sidor och skapa bokmärken eller miniatyrbilder), även om [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) är klar. |
| [getClass()](#getClass--) |  |
| [getExtractContentPermission()](#getExtractContentPermission--) | Anger om det ska tillåtas att kopiera eller på annat sätt extrahera text och grafik från dokumentet genom operationer som inte styrs av [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--). |
| [getExtractContentPermissionObsolete()](#getExtractContentPermissionObsolete--) | Tillstånd att kopiera eller extrahera innehåll har föråldrats enligt PDF-referensen. |
| [getFillFormsPermission()](#getFillFormsPermission--) | Anger om det ska tillåtas att fylla i befintliga interaktiva formulärfält (inklusive signaturfält), även om [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) är klar. |
| [getFullQualityPrintPermission()](#getFullQualityPrintPermission--) | Anger om det ska tillåtas att skriva ut dokumentet till en representation från vilken en trogen digital kopia av PDF-innehållet kan genereras. |
| [getModifyDocumentPermission()](#getModifyDocumentPermission--) | Anger om det ska tillåtas att ändra dokumentets innehåll genom operationer som inte styrs av [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) och [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--). |
| [getOwnerPassword()](#getOwnerPassword--) | Hämtar ägarlösenordet för det krypterade PDF-dokumentet. |
| [getPrintPermission()](#getPrintPermission--) | Anger om det ska tillåtas att skriva ut dokumentet. |
| [getUserPassword()](#getUserPassword--) | Hämtar användarlösenordet som krävs för att öppna det krypterade PDF-dokumentet. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAccessibilityExtractContent(boolean value)](#setAccessibilityExtractContent-boolean-) | Anger om det ska tillåtas att extrahera text och grafik (för att stödja tillgänglighet för användare med funktionsnedsättningar eller för andra ändamål). |
| [setAnnotationsPermission(boolean value)](#setAnnotationsPermission-boolean-) | Anger om det ska tillåtas att lägga till eller ändra textanteckningar, fylla i interaktiva formulärfält. |
| [setAssembleDocumentPermission(boolean value)](#setAssembleDocumentPermission-boolean-) | Anger om det ska tillåtas att montera dokumentet (infoga, rotera eller ta bort sidor och skapa bokmärken eller miniatyrbilder), även om [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) är klar. |
| [setExtractContentPermission(boolean value)](#setExtractContentPermission-boolean-) | Anger om det ska tillåtas att kopiera eller på annat sätt extrahera text och grafik från dokumentet genom operationer som inte styrs av [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--). |
| [setExtractContentPermissionObsolete(boolean value)](#setExtractContentPermissionObsolete-boolean-) | Tillstånd att kopiera eller extrahera innehåll har föråldrats enligt PDF-referensen. |
| [setFillFormsPermission(boolean value)](#setFillFormsPermission-boolean-) | Anger om det ska tillåtas att fylla i befintliga interaktiva formulärfält (inklusive signaturfält), även om [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) är klar. |
| [setFullQualityPrintPermission(boolean value)](#setFullQualityPrintPermission-boolean-) | Anger om det ska tillåtas att skriva ut dokumentet till en representation från vilken en trogen digital kopia av PDF-innehållet kan genereras. |
| [setModifyDocumentPermission(boolean value)](#setModifyDocumentPermission-boolean-) | Anger om det ska tillåtas att ändra dokumentets innehåll genom operationer som inte styrs av [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) och [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--). |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | Ställer in ägarlösenordet för det krypterade PDF-dokumentet. |
| [setPrintPermission(boolean value)](#setPrintPermission-boolean-) | Anger om det ska tillåtas att skriva ut dokumentet. |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | Ställer in användarlösenordet som krävs för att öppna det krypterade PDF-dokumentet. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfSecurityOptions() {#PdfSecurityOptions--}
```
public PdfSecurityOptions()
```


Konstruktorn för PdfSecurityOptions

**Example**

Följande kod ställer in högupplöst utskriftsbehörighet för den resulterande PDF-filen.

```
         Workbook wb = new Workbook();
         wb.getWorksheets().get(0).getCells().get("A1").setValue("Aspose");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
 
         PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();
 
         //set owner password
         pdfSecurityOptions.setOwnerPassword("YourOwnerPassword");
 
         //set user password
         pdfSecurityOptions.setUserPassword("YourUserPassword");
 
         //set print permisson
         pdfSecurityOptions.setPrintPermission(true);
 
         //set high resolution for print
         pdfSecurityOptions.setFullQualityPrintPermission(true);
 
 
         pdfSaveOptions.setSecurityOptions(pdfSecurityOptions);
 
         wb.save("output.pdf", pdfSaveOptions);
```

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAccessibilityExtractContent() {#getAccessibilityExtractContent--}
```
public boolean getAccessibilityExtractContent()
```


Anger om det ska tillåtas att extrahera text och grafik (för att stödja tillgänglighet för användare med funktionsnedsättningar eller för andra ändamål).

**Returns:**
boolean
### getAnnotationsPermission() {#getAnnotationsPermission--}
```
public boolean getAnnotationsPermission()
```


Anger om det ska tillåtas att lägga till eller ändra textanteckningar, fylla i interaktiva formulärfält.

**Remarks**

Om [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) också är aktiverad, skapa eller ändra interaktiva formulärfält (inklusive signaturfält).

**Returns:**
boolean
### getAssembleDocumentPermission() {#getAssembleDocumentPermission--}
```
public boolean getAssembleDocumentPermission()
```


Anger om det ska tillåtas att montera dokumentet (infoga, rotera eller ta bort sidor och skapa bokmärken eller miniatyrbilder), även om [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) är klar.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getExtractContentPermission() {#getExtractContentPermission--}
```
public boolean getExtractContentPermission()
```


Anger om det ska tillåtas att kopiera eller på annat sätt extrahera text och grafik från dokumentet genom operationer som inte styrs av [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--).

**Returns:**
boolean
### getExtractContentPermissionObsolete() {#getExtractContentPermissionObsolete--}
```
public boolean getExtractContentPermissionObsolete()
```


Tillstånd att kopiera eller extrahera innehåll har föråldrats enligt PDF-referensen.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ExtractContentPermission. Denna egenskap kommer att tas bort 12 månader senare från och med september 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### getFillFormsPermission() {#getFillFormsPermission--}
```
public boolean getFillFormsPermission()
```


Anger om det ska tillåtas att fylla i befintliga interaktiva formulärfält (inklusive signaturfält), även om [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) är klar.

**Returns:**
boolean
### getFullQualityPrintPermission() {#getFullQualityPrintPermission--}
```
public boolean getFullQualityPrintPermission()
```


Anger om det ska tillåtas att skriva ut dokumentet till en representation från vilken en trogen digital kopia av PDF-innehållet kan genereras.

**Remarks**

När den är klar (och [getPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getPrintPermission--) är aktiverad) begränsas utskrift till en lågkvalitativ representation av utseendet, möjligen med försämrad kvalitet.

**Returns:**
boolean
### getModifyDocumentPermission() {#getModifyDocumentPermission--}
```
public boolean getModifyDocumentPermission()
```


Anger om det ska tillåtas att ändra dokumentets innehåll genom operationer som inte styrs av [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) och [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--).

**Returns:**
boolean
### getOwnerPassword() {#getOwnerPassword--}
```
public String getOwnerPassword()
```


Hämtar ägarlösenordet för det krypterade PDF-dokumentet.

**Remarks**

Ägarlösenordet tillåter användaren att öppna ett krypterat PDF-dokument utan några angivna åtkomstrestriktioner.

**Returns:**
java.lang.String
### getPrintPermission() {#getPrintPermission--}
```
public boolean getPrintPermission()
```


Anger om det ska tillåtas att skriva ut dokumentet.

**Remarks**

Möjligen inte på högsta kvalitet, beroende på om [getFullQualityPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFullQualityPrintPermission--) också är aktiverad.

**Returns:**
boolean
### getUserPassword() {#getUserPassword--}
```
public String getUserPassword()
```


Hämtar användarlösenordet som krävs för att öppna det krypterade PDF-dokumentet.

**Remarks**

Ägarlösenordet eller användarlösenordet kommer att krävas för att öppna ett krypterat PDF-dokument för visning.

Användarlösenordet kan vara null eller en tom sträng, i så fall krävs inget lösenord från användaren när PDF-dokumentet öppnas.

Att öppna dokumentet med rätt ägarlösenord ger full åtkomst till dokumentet.

Att öppna dokumentet med rätt användarlösenord (eller öppna ett dokument som inte har något användarlösenord) ger begränsad åtkomst enligt de angivna behörigheterna.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAccessibilityExtractContent(boolean value) {#setAccessibilityExtractContent-boolean-}
```
public void setAccessibilityExtractContent(boolean value)
```


Anger om det ska tillåtas att extrahera text och grafik (för att stödja tillgänglighet för användare med funktionsnedsättningar eller för andra ändamål).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAnnotationsPermission(boolean value) {#setAnnotationsPermission-boolean-}
```
public void setAnnotationsPermission(boolean value)
```


Anger om det ska tillåtas att lägga till eller ändra textanteckningar, fylla i interaktiva formulärfält.

**Remarks**

Om [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) också är aktiverad, skapa eller ändra interaktiva formulärfält (inklusive signaturfält).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAssembleDocumentPermission(boolean value) {#setAssembleDocumentPermission-boolean-}
```
public void setAssembleDocumentPermission(boolean value)
```


Anger om det ska tillåtas att montera dokumentet (infoga, rotera eller ta bort sidor och skapa bokmärken eller miniatyrbilder), även om [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) är klar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExtractContentPermission(boolean value) {#setExtractContentPermission-boolean-}
```
public void setExtractContentPermission(boolean value)
```


Anger om det ska tillåtas att kopiera eller på annat sätt extrahera text och grafik från dokumentet genom operationer som inte styrs av [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExtractContentPermissionObsolete(boolean value) {#setExtractContentPermissionObsolete-boolean-}
```
public void setExtractContentPermissionObsolete(boolean value)
```


Tillstånd att kopiera eller extrahera innehåll har föråldrats enligt PDF-referensen.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ExtractContentPermission. Denna egenskap kommer att tas bort 12 månader senare från och med september 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFillFormsPermission(boolean value) {#setFillFormsPermission-boolean-}
```
public void setFillFormsPermission(boolean value)
```


Anger om det ska tillåtas att fylla i befintliga interaktiva formulärfält (inklusive signaturfält), även om [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) är klar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFullQualityPrintPermission(boolean value) {#setFullQualityPrintPermission-boolean-}
```
public void setFullQualityPrintPermission(boolean value)
```


Anger om det ska tillåtas att skriva ut dokumentet till en representation från vilken en trogen digital kopia av PDF-innehållet kan genereras.

**Remarks**

När den är klar (och [getPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getPrintPermission--) är aktiverad) begränsas utskrift till en lågkvalitativ representation av utseendet, möjligen med försämrad kvalitet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setModifyDocumentPermission(boolean value) {#setModifyDocumentPermission-boolean-}
```
public void setModifyDocumentPermission(boolean value)
```


Anger om det ska tillåtas att ändra dokumentets innehåll genom operationer som inte styrs av [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) och [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public void setOwnerPassword(String value)
```


Ställer in ägarlösenordet för det krypterade PDF-dokumentet.

**Remarks**

Ägarlösenordet tillåter användaren att öppna ett krypterat PDF-dokument utan några angivna åtkomstrestriktioner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setPrintPermission(boolean value) {#setPrintPermission-boolean-}
```
public void setPrintPermission(boolean value)
```


Anger om det ska tillåtas att skriva ut dokumentet.

**Remarks**

Möjligen inte på högsta kvalitet, beroende på om [getFullQualityPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFullQualityPrintPermission--) också är aktiverad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public void setUserPassword(String value)
```


Ställer in användarlösenordet som krävs för att öppna det krypterade PDF-dokumentet.

**Remarks**

Ägarlösenordet eller användarlösenordet kommer att krävas för att öppna ett krypterat PDF-dokument för visning.

Användarlösenordet kan vara null eller en tom sträng, i så fall krävs inget lösenord från användaren när PDF-dokumentet öppnas.

Att öppna dokumentet med rätt ägarlösenord ger full åtkomst till dokumentet.

Att öppna dokumentet med rätt användarlösenord (eller öppna ett dokument som inte har något användarlösenord) ger begränsad åtkomst enligt de angivna behörigheterna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

