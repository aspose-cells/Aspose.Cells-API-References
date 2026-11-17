---
title: "Classe PdfSecurityOptions"
linktitle: "PdfSecurityOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe PdfSecurityOptions. Incapsula l'oggetto che rappresenta pdfsecurityoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/pdfsecurityoptions/
---

## PdfSecurityOptions class

Opzioni per la crittografia e le autorizzazioni di accesso per un documento PDF. PDF/A non consente impostazioni di sicurezza.

```go

type PdfSecurityOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewPdfSecurityOptions](./newpdfsecurityoptions/) | Il costruttore di PdfSecurityOptions |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetUserPassword](./getuserpassword/) | Ottiene o imposta la password utente necessaria per aprire il documento PDF crittografato. |
| [SetUserPassword](./setuserpassword/) | Ottiene o imposta la password utente necessaria per aprire il documento PDF crittografato. |
| [GetOwnerPassword](./getownerpassword/) | Ottiene o imposta la password del proprietario per il documento PDF crittografato. |
| [SetOwnerPassword](./setownerpassword/) | Ottiene o imposta la password del proprietario per il documento PDF crittografato. |
| [GetPrintPermission](./getprintpermission/) | Indica se è consentita la stampa del documento. |
| [SetPrintPermission](./setprintpermission/) | Indica se è consentita la stampa del documento. |
| [GetModifyDocumentPermission](./getmodifydocumentpermission/) | Indica se è consentita la modifica del contenuto del documento mediante operazioni diverse da quelle controllate da AnnotationsPermission, FillFormsPermission e AssembleDocumentPermission. |
| [SetModifyDocumentPermission](./setmodifydocumentpermission/) | Indica se è consentita la modifica del contenuto del documento mediante operazioni diverse da quelle controllate da AnnotationsPermission, FillFormsPermission e AssembleDocumentPermission. |
| [GetAnnotationsPermission](./getannotationspermission/) | Indica se è consentito aggiungere o modificare annotazioni di testo, compilare campi di modulo interattivi. |
| [SetAnnotationsPermission](./setannotationspermission/) | Indica se è consentito aggiungere o modificare annotazioni di testo, compilare campi di modulo interattivi. |
| [GetFillFormsPermission](./getfillformspermission/) | Indica se è consentito compilare i campi di modulo interattivi esistenti (inclusi i campi firma), anche se ModifyDocumentPermission è disattivato. |
| [SetFillFormsPermission](./setfillformspermission/) | Indica se è consentito compilare i campi di modulo interattivi esistenti (inclusi i campi firma), anche se ModifyDocumentPermission è disattivato. |
| [GetExtractContentPermission](./getextractcontentpermission/) | Indica se è consentito copiare o estrarre in altro modo testo e grafica dal documento mediante operazioni diverse da quelle controllate da AccessibilityExtractContent. |
| [SetExtractContentPermission](./setextractcontentpermission/) | Indica se è consentito copiare o estrarre in altro modo testo e grafica dal documento mediante operazioni diverse da quelle controllate da AccessibilityExtractContent. |
| [GetAccessibilityExtractContent](./getaccessibilityextractcontent/) | Indica se è consentito estrarre testo e grafica (a supporto dell'accessibilità per utenti con disabilità o per altri scopi). |
| [SetAccessibilityExtractContent](./setaccessibilityextractcontent/) | Indica se è consentito estrarre testo e grafica (a supporto dell'accessibilità per utenti con disabilità o per altri scopi). |
| [GetAssembleDocumentPermission](./getassembledocumentpermission/) | Indica se è consentito assemblare il documento (inserire, ruotare o eliminare pagine e creare segnalibri o miniature), anche se ModifyDocumentPermission è disattivato. |
| [SetAssembleDocumentPermission](./setassembledocumentpermission/) | Indica se è consentito assemblare il documento (inserire, ruotare o eliminare pagine e creare segnalibri o miniature), anche se ModifyDocumentPermission è disattivato. |
| [GetFullQualityPrintPermission](./getfullqualityprintpermission/) | Indica se è consentito stampare il documento in una rappresentazione da cui potrebbe essere generata una copia digitale fedele del contenuto PDF. |
| [SetFullQualityPrintPermission](./setfullqualityprintpermission/) | Indica se è consentito stampare il documento in una rappresentazione da cui potrebbe essere generata una copia digitale fedele del contenuto PDF. |
