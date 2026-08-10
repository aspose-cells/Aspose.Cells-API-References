---
title: "VbaProject Class"
linktitle: "VbaProject"
articleTitle: "VbaProject"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents the VBA project."
type: docs
weight: 7300
url: /php/aspose.cells/vbaproject/
---

## VbaProject class

Represents the VBA project.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [IsValidSigned](#isvalidsigned) | boolean | Indicates whether the signature of VBA project is valid or not. |
| [CertRawData](#certrawdata) | byte[] | Gets certificate raw data if this VBA project is signed. |
| [Encoding](#encoding) | Encoding | Gets and sets the encoding of VBA project. |
| [Name](#name) | String | Gets and sets the name of the VBA project. |
| [IsSigned](#issigned) | boolean | Indicates whether VBAcode is signed or not. |
| [IsProtected](#isprotected) | boolean | Indicates whether this VBA project is protected. |
| [IslockedForViewing](#islockedforviewing) | boolean | Indicates whether this VBA project is locked for viewing. |
| [Modules](#modules) | VbaModuleCollection | Gets all VbaModule objects. |
| [References](#references) | VbaProjectReferenceCollection | Gets all references of VBA project. |

## Methods

| Name | Description |
| --- | --- |
| [sign](#sign) | Sign this VBA project by a DigitalSignature |
| [protect](#protect) | Protects or unprotects this VBA project.

If islockedForViewing is true, the password could not be null. |
| [copy](#copy) | Copy VBA project from other file. |
| [validatePassword](#validatepassword) | Validates protection password. |

### VbaProject.IsValidSigned property {#isvalidsigned}

Indicates whether the signature of VBA project is valid or not.

**Type:** boolean

### VbaProject.CertRawData property {#certrawdata}

Gets certificate raw data if this VBA project is signed.

**Type:** byte[]

### VbaProject.Encoding property {#encoding}

Gets and sets the encoding of VBA project.

**Type:** Encoding

### VbaProject.Name property {#name}

Gets and sets the name of the VBA project.

**Type:** String

### VbaProject.IsSigned property {#issigned}

Indicates whether VBAcode is signed or not.

**Type:** boolean

### VbaProject.IsProtected property {#isprotected}

Indicates whether this VBA project is protected.

**Type:** boolean

### VbaProject.IslockedForViewing property {#islockedforviewing}

Indicates whether this VBA project is locked for viewing.

**Type:** boolean

### VbaProject.Modules property {#modules}

Gets all VbaModule objects.

**Type:** VbaModuleCollection

### VbaProject.References property {#references}

Gets all references of VBA project.

**Type:** VbaProjectReferenceCollection

### sign(digitalSignature) {#sign}

Sign this VBA project by a DigitalSignature

| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignature | DigitalSignature | DigitalSignature |

### protect(islockedForViewing, password) {#protect}

Protects or unprotects this VBA project.

If islockedForViewing is true, the password could not be null.

| Parameter | Type | Description |
| --- | --- | --- |
| islockedForViewing | boolean | indicates whether locks project for viewing. |
| password | String | If the value is null, unprotects this VBA project, otherwise projects the this VBA project. |

### copy(source) {#copy}

Copy VBA project from other file.

| Parameter | Type | Description |
| --- | --- | --- |
| source | VbaProject |  |

### validatePassword(password) {#validatepassword}

Validates protection password.

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | the password |

**Returns:** Whether password is the protection password of this VBA project
