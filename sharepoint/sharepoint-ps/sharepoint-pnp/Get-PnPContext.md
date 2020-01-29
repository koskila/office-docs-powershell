---
external help file:
applicable: SharePoint Server 2013, SharePoint Server 2016, SharePoint Online
schema: 2.0.0
---
# Get-PnPContext

## SYNOPSIS
Returns the current context

## DESCRIPTION
Returns a Client Side Object Model context

## EXAMPLES

### ------------------EXAMPLE 1------------------
```powershell
$ctx = Get-PnPContext
```

This will put the current context in the $ctx variable.

### ------------------EXAMPLE 2------------------
```powershell
$ctx = Get-PnPContext
$site = Get-PnPTenantSite -Detailed -Url 'https://contoso.sharepoint.com/'

$site.DenyAddAndCustomizePages = [Microsoft.Online.SharePoint.TenantAdministration.DenyAddAndCustomizePagesStatus]::Disabled

$site.Update()
$ctx.ExecuteQuery()
```

This will first get the context, then get a SPSite object, enable Custom Scripts on it, and finally commit changes by calling ExecuteQuery

## OUTPUTS

### Microsoft.SharePoint.Client.ClientContext

## RELATED LINKS

[SharePoint Developer Patterns and Practices](http://aka.ms/sppnp)