# Adobe DTM Satellite Documentation 🛰

Unofficial Adobe Satellite Documentation

----

View the [Wiki](https://github.com/unofficial-adobe-dtm-documentation/adobe-dtm-satellite-docs/wiki) for examples and further reading.

Please contribute! This repository and organization needs help documenting awesome analytics products.


## Satellite API

This is an initial copy/paste of the global object.

### "Types" Glossary

The "Types" Glossary is used to clearly define parts of the API. 

- **array:** `[array]`, `[1, 2, 3]`
- **bool:** `boolean`, `true`, `false` 
- **ƒ:** `function`, `function() {}`
- **num:** `number`, `1`, `2`, `6`
- **obj:** `{object}`, `{ name: 'Randy', id: '1bd45' }`

### API 

- **initialized:** `bool` 
- **uuid:** `num`
- **dataCache:** `{obj}`
- **$data:** `ƒ (t,e,n)`
- **BaseTool:** `ƒ (t)`
- **Logger:** `{obj}`
  - outputEnabled: `bool` 
  - messages: `[array]`
  - keepLimit: `num` 
  - flushed: `bool`
  - LEVELS: `[array]`
- **QueryParams:** `{obj}`
- **URI:** `ƒ ()`
- **URL:** `ƒ ()`
- **addEventHandler:** `ƒ (t,e,n)`
- **any:** `ƒ (t,e,n)`
- **appVersion:** `"string"`
- **availableEventEmitters:** `[array]`
- **availableTools:** `{obj}`
- **backgroundTasks:** `ƒ ()`
- **basePath:**
- **bind:** `ƒ (t,e)`
- **bindEvent:** `ƒ (t,e)`
- **bindEventOnce:** `ƒ (t,e)`
- **browserInfo:** `{obj}`
  - browser: `"string"`
  - os: `"string"`
  - deviceType: `"Desktop"`
- **buildDate:** `"string"`
- **checkAsyncInclude:** `ƒ ()`
- **cleanText:** `ƒ (t)`
- **configurationSettings:** `{obj}`
  - pageLoadRules: `[array]`
  - rules: `[array]`
  - directCallRules: `[array]`
  - settings: `{obj}`
  - data: `{obj}`
- **contains:** `ƒ (t,e)`
- **containsElement:** `ƒ (t,e)`
- **cssQuery:** `ƒ (e,n)`
- **data:** `{obj}`
  - URI: `"string"` 
  - browser: `{obj}`
  - cartItems: `[array]` 
  - revenue: `"string"`
  - host: `{obj}`
- **dataCache:** `{obj}`
- **dataElementSafe:** `ƒ (t,e)`
- **dataElements:** `obj`
  - [instance name]: `{obj}` 
  - _campaign: `{obj}`, 
  - _campaignContent: `{obj}` 
  - _campaignMedium: `{obj}` 
  - _campaignSource: `{obj}`
- **detectBrowserInfo:** `ƒ ()`
- **directCallRules:** `[array]`
- **domReady:** `ƒ (t)`
- **dynamicRules:** `[array]`
- **each:** `ƒ (t,e,n)`
- **ecommerce:** `{obj}`
  - addItem: `ƒ`, 
  - addTrans: `ƒ`, 
  - trackTrans: `ƒ`
- **encodeObjectToURI:** `ƒ (t)`
- **ensureCSSSelector:** `ƒ ()`
- **equalsIgnoreCase:** `ƒ (t,e)` 
- **errors:** `[array]`
- **escapeForHtml:** `ƒ (t)`
- **escapeHtmlParams:** `ƒ (t)`
- **eventEmitterBackgroundTasks:** `ƒ ()`
- **eventEmitters:** `[array]`
- **every:** `ƒ (t,e,n)`
- **evtHandlers:** `{obj}`
- **aftertoolinit:** `[array]`
- **execute:** `ƒ (t,e,n,i)`
- **extend:** `ƒ (t,e)`
- **filter:** `ƒ (t,e,n)`
- **filterRules:** `ƒ ()`
- **find:** `ƒ (t,e,n)`
- **fireEvent**: `ƒ (t,e)`
- **fireOnceEvents:** `[array]`
- **firePageLoadEvent:** `ƒ (t)`
- **fireRule:** `ƒ (t,e,n)`
- **flushPendingCalls:** `ƒ (t)`
- **getCaseSensitivityQueryParamsMap:** `ƒ (t)`
- **getDataElement:** `ƒ (t,e,n)`
- **getElementProperty:** `ƒ (t,e)`
- **getObjectProperty:** `ƒ (t,e,n)`
- **getQueryParam:** `ƒ (t)`
- **getQueryParamCaseInsensitive:** `ƒ (t)`
- **getToolsByType:** `ƒ (t)`
- **getUniqueRuleEvents:** `ƒ () `
- **getUserAgent:** `ƒ ()`
- **getVar:** `ƒ (n,a,r)`
- **getVars:** `ƒ (t,e,n)`
- **getVisitorId:** `ƒ ()`
- **handleEvent:** `ƒ (t)`
- **handleOverrides:** `ƒ ()`
- **hasAttr:** `ƒ(t,e)`
- **hasMultipleDomains:** `ƒ ()`
- **hasSelector: `bool`
- **indexOf:** `ƒ (t,e)`
- **inherit:** `ƒ (t,e)`
- **init:** `ƒ (e)`
- **initEventEmitters:** `ƒ ()`
- **initTools:** `ƒ (t)`
- initialized:** `bool`
- **isArray:** `ƒ isArray()`
- **isHttps:** `ƒ ()`
- **isLinkTag:** `ƒ (t)`
- **isLinked:** `ƒ (t)`
- **isLinkerLink: `ƒ (t)`
- **isNaN:** `ƒ (t)`
- **isNumber:** `ƒ (t)`
- **isObject:** `ƒ (t)`
- **isOutboundLink:** `ƒ (t)`
- **isRegex:** `ƒ (t)`

## TODO

```
isRightClick
:
ƒ (t)
isRuleActive
:
ƒ (t,e)
isString
:
ƒ (t)
isSubdomainOf
:
ƒ (t,e)
isVMLPoisoned
:
ƒ (t)
keys
:
ƒ (t)
loadEventBefore
:
ƒ (t,e)
loadPrivacyManager
:
ƒ ()
loadScript
:
ƒ (t,n)
loadScriptOnce
:
ƒ (t,e)
loadScriptSync
:
ƒ (t)
loadStoredSettings
:
ƒ ()
loadedScriptRegistry
:
{}
logError
:
ƒ (t)
map
:
ƒ (t,e,n)
matchesCss
:
ƒ (n,i)
notify
:
ƒ ()
onEvent
:
ƒ (t)
pageBottom
:
ƒ ()
pageLoadPhases
:
(5) ["aftertoolinit", "pagetop", "pagebottom", "domready", "windowload"]
pageLoadRules
:
(2) [{…}, {…}]
parseQueryParams
:
ƒ (t)
poll
:
ƒ (t,e,n)
prepareLoadPrivacyManager
:
ƒ ()
preprocessArguments
:
ƒ (t,e,n,i,a)
preventDefault
:
ƒ (t)
privacyManagerParams
:
ƒ ()
propertiesMatch
:
ƒ (t,e)
publishDate
:
"2017-11-17 21:28:10 UTC"
pushAsyncScript
:
ƒ (t)
pushBlockingScript
:
ƒ (t)
readCookie
:
ƒ (t)
readStoredSetting
:
ƒ (e)
realGetDataElement
:
ƒ (e)
registerEvents
:
ƒ (t,e)
registerEventsForTags
:
ƒ (t,n)
registerNewElementsForDynamicRules
:
ƒ ()
removeCookie
:
ƒ (t)
removeEventHandler
:
ƒ (t,e,n)
replace
:
ƒ (t,e,n,i)
ruleInScope
:
ƒ (t,n)
ruleMatches
:
ƒ (t,e,n,i)
rules
:
(9) [{…}, {…}, {…}, {…}, {…}, {…}, {…}, {…}, {…}]
scriptOnLoad
:
ƒ (t,e,n)
searchVariables
:
ƒ (t,e,n)
setCookie
:
ƒ (t,n,i)
setDebug
:
ƒ (e)
setFormListeners
:
ƒ ()
setListeners
:
ƒ ()
setLocation
:
ƒ (e)
setVar
:
ƒ ()
setVideoListeners
:
ƒ ()
settings
:
{trackInternalLinks: true, libraryName: "satelliteLib-c5b57e327ddc630dcb821319b7f4c1b8e0333aaf", isStaging: false, allowGATTcalls: false, downloadExtensions: /\.(?:doc|docx|eps|jpg|png|svg|xls|ppt|pptx|pdf|xl…s|rar|exe|wma|mov|avi|wmv|mp3|wav|m4v)($|\&|\?)/i, …}
specialProperties
:
{text: ƒ, cleanText: ƒ}
stagingLibraryOverride
:
ƒ ()
stopPropagation
:
ƒ (t)
stringify
:
ƒ (t,e)
text
:
ƒ (t)
textMatch
:
ƒ (t,e)
throttle
:
ƒ (t,e)
toArray
:
ƒ (e)
tools
:
{default: y, e0207de5badfce9d70cda7078fa15003: b, 75dda97a010df6dd87bbab6db8829f0c759b8c01: w}
track
:
ƒ (t)
trim
:
ƒ (t)
unbindEvent
:
ƒ (t,e)
updateQueryParams
:
ƒ ()
uuid
:
19
values
:
ƒ (t)
visibility
:
{isHidden: ƒ, isVisible: ƒ, getHiddenProperty: ƒ, getVisibilityEvent: ƒ}
whenEvent
:
ƒ (t,e)
__proto__
:
Object
```

