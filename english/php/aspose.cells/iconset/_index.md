---
title: "IconSet Class"
linktitle: "IconSet"
articleTitle: "IconSet"
second_title: "Aspose.Cells for PHP via Java"
description: "Describe the IconSet conditional formatting rule."
type: docs
weight: 3050
url: /php/aspose.cells/iconset/
---

## IconSet class

Describe the IconSet conditional formatting rule. This conditional formatting rule applies icons to cells according to their values.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [CfIcons](#cficons) | ConditionalFormattingIconCollection | Get the ConditionalFormattingIcon from the collection |
| [Cfvos](#cfvos) | ConditionalFormattingValueCollection | Get the CFValueObjects instance. |
| [Type](#type) | Number | Get or Set the icon set type to display. Setting the type will auto check if the current Cfvos's count is accord with th |
| [IsCustom](#iscustom) | boolean | Indicates whether the icon set is custom. Default value is false. |
| [ShowValue](#showvalue) | boolean | Get or set the flag indicating whether to show the values of the cells on which this icon set is applied. Default value  |
| [Reverse](#reverse) | boolean | Get or set the flag indicating whether to reverses the default order of the icons in this icon set. Default value is fal |

### IconSet.CfIcons property {#cficons}

Get the ConditionalFormattingIcon from the collection

**Type:** ConditionalFormattingIconCollection

### IconSet.Cfvos property {#cfvos}

Get the CFValueObjects instance.

**Type:** ConditionalFormattingValueCollection

### IconSet.Type property {#type}

Get or Set the icon set type to display. Setting the type will auto check if the current Cfvos's count is accord with the new type. If not accord, old Cfvos will be cleaned and default Cfvos will be added. The value of the property is IconSetType integer constant.

**Type:** Number

### IconSet.IsCustom property {#iscustom}

Indicates whether the icon set is custom. Default value is false.

**Type:** boolean

### IconSet.ShowValue property {#showvalue}

Get or set the flag indicating whether to show the values of the cells on which this icon set is applied. Default value is true.

**Type:** boolean

### IconSet.Reverse property {#reverse}

Get or set the flag indicating whether to reverses the default order of the icons in this icon set. Default value is false.

**Type:** boolean
