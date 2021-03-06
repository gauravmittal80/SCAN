# Http Sessions #

This tool keeps track of the existing Http Sessions on a particular Site and allows the Zaproxy user to force all requests to be on a particular session. Basically, it allows the user to easily switch between user sessions on a Site and to create a new Session without "destroying" the existing ones.

It is based on the concept of Session Tokens, which are HTTP message parameters (for now only Cookies) which allow an HTTP server to connect a request message with any previous requests or data stored. In the case of Zaproxy, conceptually, session tokens have been classified into 2 categories: default session tokens and site session tokens. The default session tokens are the ones that the user can set in the [Options screen][] and are tokens that are, by default, automatically considered session tokens for any site (eg. phpsessid, jsessionid, etc). The site session tokens are a set of tokens for a particular site and are usually set up using the popup menus available in the [Params Tab][].

This tool automatically detects, using the defined session tokens or the automatically detected default session tokens, any HTTP session which exists in the communication. The detected sessions are shown in the [Http Sessions Tab][].

The user can, using the button available on the [Http Sessions Tab][], create a new session without destroying the existing one, or can force one of the sessions as 'active'. When a session is 'active', all the outbound requests sent to the corresponding Site are modified, the session tokens being set up to match the active session. In this way, the user can easily force some messages to be 'part of' a particular session and then switch and send messages on another session.

The Http Sessions tool is configured using the [Http Sessions Options screen][Options screen].

## Accessed via ##

<table> 
 <tbody>
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpUiTabsHttpsessions" rel="nofollow">Http Sessions tab</a></td> 
   <td></td> 
  </tr> 
 </tbody>
</table>

## See also ##

<table> 
 <tbody>
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpUiOverview" rel="nofollow">UI Overview</a></td> 
   <td>for an overview of the user interface</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpStartConceptsConcepts" rel="nofollow">Features</a></td> 
   <td>provided by ZAP</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpUiDialogsOptionsHttpsessions" rel="nofollow">Http Sessions Options screen</a></td> 
   <td>for an overview of the tool's Options</td> 
  </tr> 
  <tr> 
   <td>&nbsp;&nbsp;&nbsp;&nbsp;</td> 
   <td><a href="HelpUiTabsParams" rel="nofollow">Params Tab</a></td> 
   <td>for an overview of Params Tab</td> 
  </tr> 
 </tbody>
</table>


[Options screen]: HelpUiDialogsOptionsHttpsessions
[Params Tab]: HelpUiTabsParams
[Http Sessions Tab]: HelpUiTabsHttpsessions