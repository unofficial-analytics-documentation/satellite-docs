<p align="center">
  <img alt="unofficial-analytics-docs-200px" src="https://user-images.githubusercontent.com/1074042/37249693-f9b928d4-24a0-11e8-82e4-a4a50130fdae.jpg" width="100" />
</p>

----

<h1 align="center">Satellite Documentation</h1>

<p align="center">
  <a href="#satellite-api">Satellite API</a>&nbsp;&nbsp;
  <a href="#types-glossary">Types</a>&nbsp;&nbsp;
  <a href="#method-argument-glossary">Method Arguments</a>&nbsp;&nbsp;
  <a href="#api-methods-and-properties">API</a>&nbsp;&nbsp;
  <a href="/issues">Issues</a>&nbsp;&nbsp;
  <a href="/wiki">Wiki</a>
</p>

----

This repository contains _unofficial_ **Adobe DTM Satellite Library** documentation. The Satellite Library is used for [Adobe DTM](https://marketing.adobe.com/). It manages and tracks data for Adobe DTM and Adobe Analytics. If you have insight, please contribute! 

The purpose of this document is to provide a place for the DTM community to document the **`_satellite`** library and how it works—not specifically pertaining to DTM.

## Usage Guides

The list below contains guides to implement and use the **`_satellite`** on webpages. 

- **[Script loading](https://github.com/unofficial-analytics-documentation/satellite-docs/blob/master/docs/script-loading.md):** patterns for loading **`_satellite`**.


## Satellite API 🛰

Below, the **`_satellite`** API is listed out fully and there are beginning to be snippets of code on how to use the API as well as a brief description of what the code does.

----

## Types Glossary

The "Types" Glossary is used to clearly define types for each method or property of the Satellite API. 

- **array:** `[array]`
  - _examples:_ `[1, 2, 3]`
- **bool:** `boolean`
  - _examples:_ `true`, `false` 
- **ƒ:** `function`, 
  - _examples:_ `function() {}`, `() => {}`
- **num:** `number`, 
  - _examples:_ `1`, `2`, `6`
- **obj:** `{object}`, 
 - _examples:_ `{ name: 'Randy', id: '1bd45' }`

----

## Method Argument Glossary

The Method Argument Glossary is used to clearly define arguments used witin Satellite Methods. 

- **a:** array
  - _type:_ `[array]`
  - _examples:_ `[1, 2, 3]`
- **e:** event 
  - _type:_ todo
  - _examples:_ todo
- **i:** iterator
  - _type:_ todo
  - _examples:_ todo
- **n:** todo
  - _type:_ todo
  - _examples:_ todo
- **t:** `text`,
  - _type:_ `"is a string"`
  - _examples:_ "string", "this is a string"

----

## API methods and properties

- **initialized:** `bool` 
  - _example:_ `console.log(_satellite.initialized) // true`
  - describes whether `_satellite` has successfully initialized. 
- **uuid:** `num`
  - _example:_ `console.log(_satellite.uuid) // 12`
  - universally unique identifier
- **dataCache:** `{obj}`
  - _example:_ `console.log(_satellite.dataCache[1]) // {eventProcessed: true}`
  - an `[array]` of `{objects}` with stored `events`
- **$data:** `ƒ (t,e,n)`
- **BaseTool:** `ƒ (t)`
  - _example to create settings:_ `_satellite.BaseTool({ forceLowerCase: true });`
    - **note** this example could use help. 
  - _example to extend the prototype:_ `_satellite.BaseTool.stuff = 'stuff'`
  - takes in an `{argument object}` called settings for tool setting
  - Also, has helper methods bound to its prototype 
- **Logger:** `{obj}`
  - outputEnabled: `bool` 
  - messages: `[array]`
    - _example_ `console.log(_satellite.Logger.messages);`
    - Logs the state of satellite. 
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
- **fireEvent:** `ƒ (t,e)`
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
- **hasSelector:** `bool`
- **indexOf:** `ƒ (t,e)`
- **inherit:** `ƒ (t,e)`
- **init:** `ƒ (e)`
- **initEventEmitters:** `ƒ ()`
- **initTools:** `ƒ (t)`
- **initialized:** `bool`
- **isArray:** `ƒ isArray()`
- **isHttps:** `ƒ ()`
- **isLinkTag:** `ƒ (t)`
- **isLinked:** `ƒ (t)`
- **isLinkerLink:** `ƒ (t)`
- **isNaN:** `ƒ (t)`
- **isNumber:** `ƒ (t)`
- **isObject:** `ƒ (t)`
- **isOutboundLink:** `ƒ (t)`
- **isRegex:** `ƒ (t)`
- **isRightClick:** `ƒ (t)`
- **isRuleActive:** `ƒ (t,e)`
- **isString:** `ƒ (t)`
- **isSubdomainOf:** `ƒ (t,e)`
- **isVMLPoisoned:** `ƒ (t)`
- **keys:** `ƒ (t)`
- **loadEventBefore:** `ƒ (t,e)`
- **loadPrivacyManager:** `ƒ ()`
- **loadScript:** `ƒ (t,n)`
- **loadScriptOnce:** `ƒ (t,e)`
- **loadScriptSync:** `ƒ (t)`
- **loadStoredSettings:** `ƒ ()`
- **loadedScriptRegistry:** `{obj}`
- **logError:** `ƒ (t)`
- **map:** `ƒ (t,e,n)`
- **matchesCss:** `ƒ (n,i)`
- **notify:** `ƒ ()`
- **onEvent:** `ƒ (t)`
- **pageBottom:** `ƒ ()`
- **pageLoadPhases:** `[array]`
- **pageLoadRules:** `[array]`
- **parseQueryParams:** `ƒ (t)`
- **poll:** `ƒ (t,e,n)`
- **prepareLoadPrivacyManager:** `ƒ ()`
- **preprocessArguments:** `ƒ (t,e,n,i,a)`
- **preventDefault:** `ƒ (t)`
- **privacyManagerParams:** `ƒ ()`
- **propertiesMatch:** `ƒ (t,e)`
- **publishDate:** `"string"`
- **pushAsyncScript:** `ƒ (t)`
- **pushBlockingScript:** `ƒ (t)`
- **readCookie:** `ƒ (t)`
- **readStoredSetting:** `ƒ (e)`
- **realGetDataElement:** `ƒ (e)`
- **registerEvents:** `ƒ (t,e)`
- **registerEventsForTags:** `ƒ (t,n)`
- **registerNewElementsForDynamicRules:** `ƒ ()`
- **removeCookie:** `ƒ (t)`
- **removeEventHandler:** `ƒ (t,e,n)`
- **replace:** ƒ (t,e,n,i)
- **ruleInScope:** `ƒ (t,n)`
- **ruleMatches:** `ƒ (t,e,n,i)`
- **rules:** `[array]`
- **scriptOnLoad:** `ƒ (t,e,n)`
- **searchVariables:** `ƒ (t,e,n)`
- **setCookie:** `ƒ (t,n,i)`
- **setDebug:** `ƒ (e)`
- **setFormListeners:** `ƒ ()`
- **setListeners:** `ƒ ()`
- **setLocation:** `ƒ (e)`
- **setVar:** `ƒ ()`
  - _example:_ `_satellite.setVar('PageName','test' ); _satellite.data.customVars // is an {object}`
  - [reference link](https://forums.adobe.com/thread/2422290)
- **setVideoListeners:** `ƒ ()`
- **settings:** `{obj}`
  - trackInternalLinks: `bool` 
  - libraryName: `"string"` 
  - isStaging: `bool` 
    - _example:_ `console.log(_satellite.settings.isStaging) // faulse
    - communicates which environment is being loaded w/o DOM awareness
  - allowGATTcalls: `bool`
  - downloadExtensions: `regex`
- **specialProperties** `{obj}`
  - text: `ƒ` 
  - cleanText: `ƒ`
- **stagingLibraryOverride:** `ƒ ()`
- **stopPropagation:** `ƒ (t)`
- **stringify:** `ƒ (t,e)`
- **text:** `ƒ (t)`
- **textMatch:** `ƒ (t,e)`
- **throttle:** `ƒ (t,e)`
- **toArray:** `ƒ (e)`
- **tools:** `{obj}`
- **track:** `ƒ (t)`
- **trim:** `ƒ (t)`
- **unbindEvent:** `ƒ (t,e)`
- **updateQueryParams:** `ƒ ()`
- **uuid:** `num`
- **values:** `ƒ (t)`
- **visibility:** `{obj}`
  - isHidden: `ƒ`, 
  - isVisible: `ƒ`, 
  - getHiddenProperty: `ƒ`, 
  - getVisibilityEvent: `ƒ`
- **whenEvent:** `ƒ (t,e)`
- **__proto__:** `{obj}`

