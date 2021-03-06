---
title: AppDomains element in the manifest file
description: ''
ms.date: 12/13/2018
localization_priority: Normal
---

# AppDomains element

Lists any domains in addition to the domain specified in the SourceLocation element that your Office Add-in will use to load pages. For each additional domain, specify an AppDomain element.

 **Add-in type:** Content, Task pane, Mail

## Syntax

```XML
<AppDomains>
    <AppDomain>AppDomain1</AppDomain>
    <AppDomain>AppDomain2</AppDomain>
</AppDomains>
```

> [!IMPORTANT]
> The value of each **AppDomain** element must include the protocol (e.g., `<AppDomain>https://myappdomain<AppDomain>`).

## Contained in

[OfficeApp](officeapp.md)

## Can contain

[AppDomain](appdomain.md)

## Remarks

By default, your add-in can load any page that is in the same domain as the location specified in the [SourceLocation element](sourcelocation.md). To load pages that are not in the same domain as the add-in, specify their domains by using the **AppDomains** and **AppDomain** elements. This element can't be empty.
