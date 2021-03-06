# Release 1.2.0 #

The following changes were made in this release:

## Significant changes: ##

### Memory Leaks ###

Memory leaks have been fixed in the [active scanner][] and [spider][].

### Invoke applications ###

External applications can now be invoked from the Sites and History tabs.

### Passive Scanner ###

The [passive scanner][] now looks for vulnerabilities, such as:

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Autocomplete forms with password fields</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Cookies without the 'HttpOnly' flag</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>SSL Cookies without the 'secure' flag</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td>Weak authentication</td>
  </tr> 
 </tbody>
</table>

## Minor changes: ##

### XML Reports ###

A new 'Generate XML Report...' menu item is now included in the top level [Reports][] menu.

### Manual Request Editor and Resend dialogs ###

Requests submitted by the [Manual Request Editor][] and [Resend][] dialogs are now shown in the [Sites][] and [History][] tabs.
A new 'Method' pull down allows you to switch between the HTTP methods, this automatically moves parameters between the URL and the body when a POST method is selected or deselected.

### Alerts UI ###

The [Sites][] tab now shows any alerts as flags to the right of any node names.
The alert counts in the [footer][] now show the number of different types of alerts rather than the total number of instances.

### Active scanner delay option ###

The delay in milliseconds between each [active scanner][] request can now be set via the [Options Active Scan screen][]. This will increase the time an active scan takes but will reduce the load on the target.

### UI Changes ###

The [Sites][] tab now takes up all of the left hand side - this can be changed back via the [Options Display screen][Options Active Scan screen] if required.

The 'toolbar' on the [Request][], [Response][] and [Break][] tabs and the [Manual Request Editor][] and [Resend][] dialogs is now at the top rather than the bottom.

The scanner counts in the [footer][] are now displayed on the right hand side.



## See also ##

<table> 
 <tbody>
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpIntro" rel="nofollow">Introduction</a></td>
   <td>the introduction to ZAP</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpReleasesReleases" rel="nofollow">Releases</a></td>
   <td>the full set of releases</td>
  </tr> 
  <tr>
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td>
   <td> <a href="HelpCredits" rel="nofollow">Credits</a></td>
   <td>the people and groups who have made this release possible</td>
  </tr> 
 </tbody>
</table>


[active scanner]: HelpStartConceptsAscan
[spider]: HelpStartConceptsSpider
[passive scanner]: HelpStartConceptsPscan
[Reports]: HelpUiTlmenuReport
[Manual Request Editor]: HelpUiDialogsMan_req
[Resend]: HelpUiDialogsResend
[Sites]: HelpUiTabsSites
[History]: HelpUiTabsHistory
[footer]: HelpUiFooter
[Options Active Scan screen]: HelpUiDialogsOptionsAscan
[Request]: HelpUiTabsRequest
[Response]: HelpUiTabsResponse
[Break]: HelpUiTabsBreak