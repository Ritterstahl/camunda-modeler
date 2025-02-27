# Changelog

All notable changes to the [Camunda Modeler](https://github.com/camunda/camunda-modeler) are documented here. We use [semantic versioning](http://semver.org/) for releases.

## Unreleased

___Note:__ Yet to be released changes appear here._

## 5.2.0

### General

* `FEAT`: toggle properties panel errors when toggling error panel ([#3014](https://github.com/camunda/camunda-modeler/pull/3014))
* `FIX`: fix error panel styles ([#3015](https://github.com/camunda/camunda-modeler/pull/3015))
* `FIX`: load modeling styles globally ([#3031](https://github.com/camunda/camunda-modeler/pull/3031))
* `FIX`: fix PNG export on DRD diagrams ([#3068](https://github.com/camunda/camunda-modeler/issues/3068))
* `DEPS`: bump @camunda/linting to v0.3.4 ([#3065](https://github.com/camunda/camunda-modeler/pull/3065))
* `DEPS`: bump diagram-js to v8.7.1 ([#3065](https://github.com/camunda/camunda-modeler/pull/3065))
* `DEPS`: bump diagram-js-direct-editing to v1.7.0 ([#3065](https://github.com/camunda/camunda-modeler/pull/3065))
* `DEPS`: bump diagram-js-origin to v1.3.3 ([#3065](https://github.com/camunda/camunda-modeler/pull/3065))
* `DEPS`: bump min-dom to v3.2.1 ([#3065](https://github.com/camunda/camunda-modeler/pull/3065))


### BPMN
* `FEAT`: add FEEL editor for FEEL properties ([#158](https://github.com/bpmn-io/properties-panel/pull/158))
* `FIX`: check for replacement using actual target ([#1699](https://github.com/bpmn-io/bpmn-js/pull/1699))
* `FIX`: do not update empty business key ([#2](https://github.com/camunda/camunda-bpmn-js-behaviors/pull/2))
* `DEPS`: bump bpmn-js to v9.3.2 ([#3065](https://github.com/camunda/camunda-modeler/pull/3065))
* `DEPS`: bump camunda-bpmn-js to v0.16.1 ([#3065](https://github.com/camunda/camunda-modeler/pull/3065))

### DMN

* `FIX`: attach and detach DMN overview properly ([#3080](https://github.com/camunda/camunda-modeler/pull/3080))

## 5.1.0

_Adds a multi-element context, improves overall selection UX in diagram editors, and ships conditional element template properties (C8 only)._

### General

* `CHORE`: mask non-boolean flag values for ping event ([#2963](https://github.com/camunda/camunda-modeler/pull/2963))
* `CHORE`: track set flags via ping event ([#2963](https://github.com/camunda/camunda-modeler/pull/2963))
* `CHORE`: use @camunda/linting ([#2976](https://github.com/camunda/camunda-modeler/pull/2976))
* `CHORE`: implement mixpanel telemetry ([#2934](https://github.com/camunda/camunda-modeler/issues/2934))
* `FIX`: debounced input fields no longer lose their values ([#2990](https://github.com/camunda/camunda-modeler/issues/2990))
* `FIX`: always write file when save is triggered ([#2925](https://github.com/camunda/camunda-modeler/issues/2925))
* `FIX`: explicitly specify default credentials during deploy ([#2924](https://github.com/camunda/camunda-modeler/pull/2924))
* `FIX`: reverse order of input error and description during deploy ([#2918](https://github.com/camunda/camunda-modeler/issues/2918))
* `FIX`: make sorting of error diagram errors deterministic ([#2933](https://github.com/camunda/camunda-modeler/pull/2933))
* `FIX`: disable reopen last tab on empty start ([#2893](https://github.com/camunda/camunda-modeler/pull/2893))
* `FIX`: adjust overlay max heights to alway fit viewport ([#2915](https://github.com/camunda/camunda-modeler/pull/2915))
* `FIX`: use separate linting state ([#2917](https://github.com/camunda/camunda-modeler/pull/2917))
* `FIX`: add form-js notice to license ([#2947](https://github.com/camunda/camunda-modeler/pull/2947))
* `FIX`: improved file dialogs to match OS defaults ([#2300](https://github.com/camunda/camunda-modeler/issues/2300), [#2971](https://github.com/camunda/camunda-modeler/pull/2971))
* `FIX`: reorder close file dialog buttons to match convention ([#2895](https://github.com/camunda/camunda-modeler/pull/2895))
* `CHORE`: configure process env for mixpanel ([#2941](https://github.com/camunda/camunda-modeler/pull/2941))
* `CHORE`: removed 'new' badge for C8 ([#2953](https://github.com/camunda/camunda-modeler/issues/2953)) 
* `DEPS`: bump electron to 19.0.6 ([#2998](https://github.com/camunda/camunda-modeler/pull/2998), [#3004](https://github.com/camunda/camunda-modeler/pull/3004))
* `DEPS`: bump properties-panel to 1.2.0 ([bc8b74870](https://github.com/camunda/camunda-modeler/commit/bc8b74870))
* `DEPS`: bump diagram-js to 8.7.0 ([bc8b74870](https://github.com/camunda/camunda-modeler/commit/bc8b74870))

### BPMN

* `FEAT`: allow to select participant and subprocess via click on body ([bpmn-js#1646](https://github.com/bpmn-io/bpmn-js/pull/1646))
* `FEAT`: add multi-element context pad ([bpmn-js#1525](https://github.com/bpmn-io/bpmn-js/pull/1525))
* `FEAT`: add aligment and distribution menu ([bpmn-js#1680](https://github.com/bpmn-io/bpmn-js/issues/1680), [camunda-bpmn-js#1691](https://github.com/bpmn-io/bpmn-js/issues/1691))
* `FEAT`: rework diagram interaction handles ([diagram-js#640](https://github.com/bpmn-io/diagram-js/pull/640))
* `FEAT`: rework select and hover interaction on the diagram ([bpmn-js#1616](https://github.com/bpmn-io/bpmn-js/issues/1616), [diagram-js#640](https://github.com/bpmn-io/diagram-js/pull/640), [diagram-js#643](https://github.com/bpmn-io/diagram-js/pull/643))
* `FEAT`: enable multi-select state in properties panel ([bpmn-props-panel#687](https://github.com/bpmn-io/bpmn-js-properties-panel/pull/678))
* `FEAT`: display timestamp for template versions ([bpmn-props-panel#698](https://github.com/bpmn-io/bpmn-js-properties-panel/pull/698))
* `FIX`: added separator to process variable sources ([#3003](https://github.com/camunda/camunda-modeler/issues/3003))
* `FIX`: editing field injections no longer crashes the modeler ([#2989](https://github.com/camunda/camunda-modeler/issues/2989))
* `FIX`: element template name and icon now display properly on versioned templates ([#2920](https://github.com/camunda/camunda-modeler/issues/2920))
* `FIX`: collapsing subprocesses correctly handles sequence flow labels ([#2993](https://github.com/camunda/camunda-modeler/issues/2993))
* `FIX`: use explicit `Decision ID` label for called decisions ([#2725](https://github.com/camunda/camunda-modeler/issues/2725))
* `FIX`: complete direct editing on selection changed ([#2961](https://github.com/camunda/camunda-modeler/issues/2961))
* `FIX`: lint subscriptions only if start event is child to a subprocess ([#2983](https://github.com/camunda/camunda-modeler/issues/2983))
* `FIX`: cancel direct editing before shape deletion ([bpmn-js#1677](https://github.com/bpmn-io/bpmn-js/issues/1677))
* `DEPS`: bump camunda-bpmn-js to 0.15.2 ([bc8b74870](https://github.com/camunda/camunda-modeler/commit/bc8b74870), [dbe78ef45](https://github.com/camunda/camunda-modeler/commit/dbe78ef45))
* `DEPS`: bump bpmn-js-properties-panel to 1.2.0 ([bc8b74870](https://github.com/camunda/camunda-modeler/commit/bc8b74870))
* `DEPS`: bump bpmn-js to 9.3.1 ([bc8b74870](https://github.com/camunda/camunda-modeler/commit/bc8b74870))
* `DEPS`: bump bpmnlint-plugin-camunda-compat to 0.9.1 ([#2927](https://github.com/camunda/camunda-modeler/issues/2927), [d6cc308](https://github.com/camunda/camunda-modeler/commit/d6cc308))

### DMN

* `FEAT`: rework diagram interaction handles ([diagram-js#640](https://github.com/bpmn-io/diagram-js/pull/640))
* `FEAT`: rework select and hover interaction on the diagram ([diagram-js#640](https://github.com/bpmn-io/diagram-js/pull/640), [diagram-js#643](https://github.com/bpmn-io/diagram-js/pull/643))
* `FIX`: allow to scroll variable type in literal expression ([#2908](https://github.com/camunda/camunda-modeler/issues/2908))
* `DEPS`: bump dmn-js to 12.2.0 ([#3019](https://github.com/camunda/camunda-modeler/pull/3019))
* `DEPS`: bump camunda-dmn-js to 0.5.0 ([#3019](https://github.com/camunda/camunda-modeler/pull/3019))
* `DEPS`: bump dmn-js-properties-panel to 1.1.0 ([#3019](https://github.com/camunda/camunda-modeler/pull/3019))


### Forms

* `FIX`: textfield 'regularExpressionPattern' now correctly sets 'pattern' in the form definition ([#2919](https://github.com/camunda/camunda-modeler/issues/2919))
* `DEPS`: bump form-js from 0.7.0 to 0.7.2 ([15aed67091](https://github.com/camunda/camunda-modeler/commit/15aed67091))

## 5.0.0

### General

* `FEAT`: update app icon ([#2875](https://github.com/camunda/camunda-modeler/pull/2875))
* `FEAT`: overhaul the welcome page design and add `new` badge for Camunda Platform 8 ([#2829](https://github.com/camunda/camunda-modeler/pull/2829) and [#2830](https://github.com/camunda/camunda-modeler/issues/2830))
* `FEAT`: rename Camunda Platform to Camunda Platform 7 and Camunda Cloud to Camunda Platform 8 ([`129af3`](https://github.com/camunda/camunda-modeler/commit/129af3c14ba81a4dd21de6210240c58eee35ca77), [`33e5e8`](https://github.com/camunda/camunda-modeler/commit/33e5e86990274c590fadc3c508c1b27cda900ff2), [`673293`](https://github.com/camunda/camunda-modeler/commit/67329359a19be2cd5335499b941d05218631467e), [`86ccec`](https://github.com/camunda/camunda-modeler/commit/86ccec8dd7e70c80da7454f863816ed06f5990d5), and [#2834](https://github.com/camunda/camunda-modeler/issues/2834))
* `FEAT`: add Camunda Platform 8 and Camunda Platform 7.17 in platform version selector ([#2736](https://github.com/camunda/camunda-modeler/issues/2736))
* `FEAT`: link to new docs homepage ([`d036a0`](https://github.com/camunda/camunda-modeler/commit/d036a0a520b7ff4b68dcd74575fc4d29b39dd4f6), [`555abb`](https://github.com/camunda/camunda-modeler/commit/555abb368880f5d631d461b0d109a749ef880d65), and [`d92633`](https://github.com/camunda/camunda-modeler/commit/d92633eeaf5b97f8bf699d81821991612e2522cd))
* `FEAT`: add display-version flag ([#2790](https://github.com/camunda/camunda-modeler/issues/2790) and [`5ca662`](https://github.com/camunda/camunda-modeler/commit/5ca6621848d7b314eb56f6fc96a98d7b72f9ecc2))
* `FEAT`: send telemetry data for usage of plugins ([#2818](https://github.com/camunda/camunda-modeler/issues/2818))
* `FEAT`: send telemetry data for button/link clicks on welcome page ([#2828](https://github.com/camunda/camunda-modeler/issues/2828))
* `FIX`: always show active tab indicator ([#2732](https://github.com/camunda/camunda-modeler/issues/2732))
* `FIX`: avoid error when closing startInstance overlay via canvas click ([#2727](https://github.com/camunda/camunda-modeler/issues/2727))
* `FIX`: log errors in context of toast notifications ([#2793](https://github.com/camunda/camunda-modeler/issues/2793))
* `FIX`: don't open external links twice in some situations ([#2905](https://github.com/camunda/camunda-modeler/issues/2905))
* `CHORE`: add query parameters to external camunda.com and camunda.io links ([`0708ac`](https://github.com/camunda/camunda-modeler/commit/0708ace145056e7d3dbf35dab492651036a919d6))
* `DEPS`: bump to `electron@17.1.0` ([#2797](https://github.com/camunda/camunda-modeler/pull/2797))
* `DEPS`: bump to `zeebe-node@2.1.0` ([#2783](https://github.com/camunda/camunda-modeler/issues/2783))

### BPMN

* `FEAT`: add element template support for Camunda Platform 8 BPMN diagrams ([#2785](https://github.com/camunda/camunda-modeler/pull/2785))
* `FEAT`: allow configuration of custom groups for element template configurations ([#2673](https://github.com/camunda/camunda-modeler/issues/2673))
* `FEAT`: send telemetry data for usage of element templates used for Camunda Platform 8 BPMN diagrams ([#2786](https://github.com/camunda/camunda-modeler/issues/2786), and [`268c53`](https://github.com/camunda/camunda-modeler/commit/268c53b00f9bd75055dfddf9683ba603c5c7337d))
* `FEAT`: make deploy to Camunda Platform 8 SaaS the default selection in deploy tool ([#2832](https://github.com/camunda/camunda-modeler/issues/2832))
* `FEAT`: show error in properties panel on click on respective error ([#2861](https://github.com/camunda/camunda-modeler/pull/2861))
* `FEAT`: add implementation level validation and respective errors ([#2891](https://github.com/camunda/camunda-modeler/pull/2891))
* `FEAT`: improve UI of deploy tool ([#2863](https://github.com/camunda/camunda-modeler/issues/2863), and [#2860](https://github.com/camunda/camunda-modeler/issues/2860))
* `FEAT`: let plugins differentiate between BPMN tabs for either cloud, platform, or both ([#2757](https://github.com/camunda/camunda-modeler/issues/2757))
* `FEAT`: pick up `bpmn-js` and `moddle` plugins for cloud BPMN tabs ([#2766](https://github.com/camunda/camunda-modeler/issues/2766))
* `FEAT`: send telemetry data for usage of collapsed subprocesses ([#2756](https://github.com/camunda/camunda-modeler/issues/2756))
* `FIX`: show properties-panel icon for ad-hoc subProcess ([#2749](https://github.com/camunda/camunda-modeler/issues/2749))
* `FIX`: make labels for formType selection in properties panel easier to understand ([#2496](https://github.com/camunda/camunda-modeler/issues/2496))
* `FIX`: avoid error in deployPlugin when file menu is used ([#2762](https://github.com/camunda/camunda-modeler/issues/2762))
* `FIX`: allow copy&paste of linting errors on MacOS ([#2716](https://github.com/camunda/camunda-modeler/issues/2716))
* `FIX`: correctly show color icons in edit > color menu ([#2733](https://github.com/camunda/camunda-modeler/issues/2733))
* `FIX`: show variableName and variableEvents for Conditional Events ([#2866](https://github.com/camunda/camunda-modeler/issues/2866))
* `FIX`: correctly persist Message End Events with external task configuration to XML ([#2865](https://github.com/camunda/camunda-modeler/issues/2865))
* `DEPS`: bump to `bpmn-js-properties-panel@1.0.0-alpha.12` ([`b3ec90`](https://github.com/camunda/camunda-modeler/commit/b3ec90616543816a38fac1ef87dbf93f0c286738))
* `DEPS`: bump to `camunda-bpmn-js@0.13.0-alpha.8` ([`b3ec90`](https://github.com/camunda/camunda-modeler/commit/b3ec90616543816a38fac1ef87dbf93f0c286738))
* `DEPS`: bump to `diagram-js@8.2.1` ([`b3ec90`](https://github.com/camunda/camunda-modeler/commit/b3ec90616543816a38fac1ef87dbf93f0c286738))
* `DEPS`: bump to `zeebe-bpmn-moddle@0.12.1` ([`b3ec90`](https://github.com/camunda/camunda-modeler/commit/b3ec90616543816a38fac1ef87dbf93f0c286738))

### DMN

* `FEAT`: add DMN modeler for Camunda Platform 8 ([#2525](https://github.com/camunda/camunda-modeler/issues/2525))
* `FEAT`: add deploy tool for Camunda Platform 8 DMN diagrams ([#2526](https://github.com/camunda/camunda-modeler/issues/2526))
* `FEAT`: let plugins differentiate between DMN tabs for either cloud, platform, or both ([#2854](https://github.com/camunda/camunda-modeler/issues/2854))
* `FEAT`: support engine profile selection for DMN diagrams ([#2872](https://github.com/camunda/camunda-modeler/issues/2872))
* `FEAT`: send telemetry data for engine usage within DMN diagrams on diagramOpen or diagramDeploy ([#2853](https://github.com/camunda/camunda-modeler/issues/2853))
* `FIX`: allow opening of DMN 1.3 files with xml file extension ([#2841](https://github.com/camunda/camunda-modeler/issues/2841))
* `DEPS`: add `camunda-dmn-js@0.2.2` ([`ba3a6c`](https://github.com/camunda/camunda-modeler/commit/ba3a6cc00b3b68d5be718f35ec927ed439c67c4f))
* `DEPS`: bump to `dmn-js@12.1.0` ([`ba3a6c`](https://github.com/camunda/camunda-modeler/commit/ba3a6cc00b3b68d5be718f35ec927ed439c67c4f))

### Forms

* `DEPS`: bump to form-js@0.7.0 ([`3a20df`](https://github.com/camunda/camunda-modeler/commit/3a20df7a61d4fa498e250c8ae31ebc62b51a50f5))

### Breaking Changes

* `Camunda Platform` is now consistenly labeled as `Camunda Platform 7` and `Camunda Cloud` as `Camunda Platform 8`. This is a UI-level change and diagram data is not affected.

## 5.0.0-alpha.1

### BPMN
* `FEAT`: support drilldown into subprocesses ([#1443](https://github.com/bpmn-io/bpmn-js/issues/1443))
* `FEAT`: support linting in platform diagrams ([#2625](https://github.com/camunda/camunda-modeler/issues/2625))
* `FEAT`: track userTask formRef usage ([#2737](https://github.com/camunda/camunda-modeler/pull/2737))

## 5.0.0-alpha.0

### General

* `FEAT`: track Camunda Platform as target type in telemetry ([#2238](https://github.com/camunda/camunda-modeler/issues/2238))
* `FEAT`: expose properties panel library to plugins ([#2632](https://github.com/camunda/camunda-modeler/pull/2632))
* `FEAT`: redesign properties panel handle bar ([#2633](https://github.com/camunda/camunda-modeler/issues/2633))
* `FEAT`: add tab context menu ([#2630](https://github.com/camunda/camunda-modeler/issues/2630), [#1240](https://github.com/camunda/camunda-modeler/issues/1240))
* `FEAT`: redesign the notifications ([#2607](https://github.com/camunda/camunda-modeler/issues/2607), [#2643](https://github.com/camunda/camunda-modeler/issues/2643))
* `FEAT`: add new file button with keyboard shortcut and navigation ([#2556](https://github.com/camunda/camunda-modeler/issues/2556), [#2626](https://github.com/camunda/camunda-modeler/issues/2626))
* `FEAT`: remove toolbar ([#2569](https://github.com/camunda/camunda-modeler/issues/2569))
* `FEAT`: redesign the tab container ([#2562](https://github.com/camunda/camunda-modeler/issues/2562))
* `FEAT`: redesign and improve UX of the status bar ([#2488](https://github.com/camunda/camunda-modeler/issues/2488))
* `FEAT`: increase default window size ([`9a00eff`](https://github.com/camunda/camunda-modeler/commit/9a00effc4c7d3a5c1b06280ea11add4ca7b2ede5))
* `FEAT`: implement reduced color scheme ([#2459](https://github.com/camunda/camunda-modeler/issues/2459)), ([#2550](https://github.com/camunda/camunda-modeler/issues/2550))
* `FEAT`: redesign the tab bar ([#2507](https://github.com/camunda/camunda-modeler/issues/2507), [#2563](https://github.com/camunda/camunda-modeler/issues/2563), [#2440](https://github.com/camunda/camunda-modeler/issues/2440))
* `FEAT`: allow to drop files from VSCode ([#2299](https://github.com/camunda/camunda-modeler/issues/2299))
* `FEAT`: expose Overlay component ([#2492](https://github.com/camunda/camunda-modeler/pull/2492))
* `FEAT`: make file permissions for Linux more strict ([#2439](https://github.com/camunda/camunda-modeler/issues/2439))
* `FEAT`: improve welcome tab UI ([#2470](https://github.com/camunda/camunda-modeler/issues/2470), [#2479](https://github.com/camunda/camunda-modeler/issues/2479))
* `FIX`: restrict height of log ([#2258](https://github.com/camunda/camunda-modeler/issues/2258))
* `FIX`: require at least one item of system information to be checked ([#2414](https://github.com/camunda/camunda-modeler/issues/2414))
* `DEPS`: update to `electron@12.1.2`

### BPMN

* `FEAT`: support Camunda Cloud 1.4 ([#2524](https://github.com/camunda/camunda-modeler/issues/2524), [#2641](https://github.com/camunda/camunda-modeler/issues/2641))
* `FEAT`: UX and technical re-write of the properties panel for Camunda Platform diagrams  ([#2663](https://github.com/camunda/camunda-modeler/issues/2663))
* `FEAT`: validate diagrams ([#2466](https://github.com/camunda/camunda-modeler/issues/2466), [#2464](https://github.com/camunda/camunda-modeler/issues/2464))
* `FEAT`: allow to pass variables when starting an instance ([#2437](https://github.com/camunda/camunda-modeler/issues/2437))
* `FEAT`: allow to set execution platform version ([#2465](https://github.com/camunda/camunda-modeler/issues/2465))
* `FEAT`: move color picker to the edit menu ([#2568](https://github.com/camunda/camunda-modeler/issues/2568))
* `FEAT`: use text area for form JSON configuration in Camunda Cloud diagram ([#2579](https://github.com/camunda/camunda-modeler/issues/2579))
* `FEAT`: add `--disable-platform` flag which allows to disable Camunda Platform features ([#2506](https://github.com/camunda/camunda-modeler/issues/2506))
* `FEAT`: use overlay for deploy and start instance tools ([#2489](https://github.com/camunda/camunda-modeler/issues/2489))
* `FIX`: do not display compensation SubProcess in the list of activities to be compensated ([#2397](https://github.com/camunda/camunda-modeler/issues/2397))
* `FIX`: rename "Target" to "Called element" for Camunda Cloud Call Activity ([#2586](https://github.com/camunda/camunda-modeler/issues/2586))
* `FIX`: keep properties panel updated when root changes ([[#2374](https://github.com/camunda/camunda-modeler/issues/2374))
* `FIX`: set correct attributes when coloring connections ([#2599](https://github.com/camunda/camunda-modeler/issues/2599))
* `FIX`: show proper tooltip on start instance tool ([#2429](https://github.com/camunda/camunda-modeler/issues/2429))
* `DEPS`: update to `bpmn-js@8.9.1`

### DMN

* `FIX`: keep selection of a replaced element ([#2306](https://github.com/camunda/camunda-modeler/issues/2306))
* `DEPS`: update to `dmn-js@11.1.2`

### Forms

* `FEAT`: split Camunda Platform and Camunda Cloud forms ([#2650](https://github.com/camunda/camunda-modeler/issues/2650))
* `FEAT`: allow to deploy Camunda Platform forms ([#2498](https://github.com/camunda/camunda-modeler/issues/2498))
* `FEAT`: allow to drag and drop forms ([#2490](https://github.com/camunda/camunda-modeler/issues/2490))
* `FIX`: properly set exporter metadata ([#2540](https://github.com/camunda/camunda-modeler/issues/2540))
* `FIX`: enable "Select all" in properties panel ([#2411](https://github.com/camunda/camunda-modeler/issues/2411))
* `FIX`: do not disable save options when tab is switched ([#2635](https://github.com/camunda/camunda-modeler/issues/2635))
* `FIX`: make sure select component can be selected via click ([#2415](https://github.com/camunda/camunda-modeler/issues/2415))
* `DEPS`: update to `@bpmn-io/form-js@0.6.0`

### Breaking Changes

* The properties panel extensions for `0.x` series don't work with the new properties panel. Check out [the project's changelog](https://github.com/bpmn-io/bpmn-js-properties-panel/blob/master/CHANGELOG.md#breaking-changes) with the example migration for guidance.
* The `toolbar` slot has been removed. Consider moving your plugin's buttons to the status bar. Check out [the `how to migrate your Camunda Modeler plugin` blog post](https://camunda.com/blog/2022/01/how-to-migrate-your-camunda-modeler-plugins-to-work-with-camunda-modeler-5-x/) for guidance.

## 4.12.0

* `FEAT`: define engine profiles globally ([#2544](https://github.com/camunda/camunda-modeler/issues/2544))
* `FEAT`: support Zeebe 1.3 / Camunda Cloud 1.3 ([#2578](https://github.com/camunda/camunda-modeler/issues/2578), [#2535](https://github.com/camunda/camunda-modeler/issues/2535))
* `FIX`: keep original IDs when copy and pasting elements between diagrams ([#1410](https://github.com/camunda/camunda-modeler/issues/1410))
* `FIX`: hide disabled engines in Form Editor select ([#2512](https://github.com/camunda/camunda-modeler/issues/2512))
* `DEPS`: update to `bpmn-js@8.8.2`

## 4.11.1

* `FIX`: correct deployment of Camunda Forms with `camunda:formRefBinding=latest` ([#2484](https://github.com/camunda/camunda-modeler/issues/2484))
* `FIX`: quit application on MacOS when forcefully requested ([#1803](https://github.com/camunda/camunda-modeler/issues/1803))

## 4.11.0

### General

* `FEAT`: support Zeebe 1.2 / Camunda Cloud 1.2 ([#2423](https://github.com/camunda/camunda-modeler/issues/2423), [#2428](https://github.com/camunda/camunda-modeler/issues/2428), [#2420](https://github.com/camunda/camunda-modeler/issues/2420))
* `FEAT`: support for Camunda Platform 7.16 ([#2428](https://github.com/camunda/camunda-modeler/issues/2428), [#2295](https://github.com/camunda/camunda-modeler/issues/2295))
* `FIX`: link to correct timer event documentation ([#2413](https://github.com/camunda/camunda-modeler/issues/2413))

### BPMN
* `FEAT`: allow Form reference bindings for User Tasks and Start Events ([#2295](https://github.com/camunda/camunda-modeler/issues/2295))
* `FIX`: allow deployment to Camunda Platform version 7.8.0 and below ([#2340](https://github.com/camunda/camunda-modeler/issues/2340))

## 4.10.0

### General

* `FEAT`: add `Provide Feedback` button in the status bar, allowing to copy system information to clipboard ([#2388](https://github.com/camunda/camunda-modeler/issues/2388))
* `FEAT`: add context action to tabs to reveal respective file in file explorer ([#1834](https://github.com/camunda/camunda-modeler/issues/1834))
* `FIX`: disable editor shortcuts when developer tools are open ([#2389](https://github.com/camunda/camunda-modeler/issues/2389))
* `FIX`: ensure that user retrieves an update notification when using the manual `Check for Updates` action by not using the staged rollout mechanism ([#2263](https://github.com/camunda/camunda-modeler/issues/2263))
* `FIX`: keep tab open when a save dialog was canceled ([#2359](https://github.com/camunda/camunda-modeler/issues/2359))

### BPMN

* `FEAT`: UX and technical re-write of the Properties Panel for Camunda Cloud diagrams ([#2347](https://github.com/camunda/camunda-modeler/issues/2347))
* `FEAT`: allow the user to deploy diagrams to different Camunda Cloud regions by using the Cluster URL (instead of Cluster ID) ([#2375](https://github.com/camunda/camunda-modeler/issues/2375))
* `FIX`: correctly encode Camunda-Forms inside UserTasks ([#2365](https://github.com/camunda/camunda-modeler/issues/2365))
* `DEPS`: update to `bpmn-js@8.7.3`

### DMN

* `FIX`: display edit cell button in decision table view in correct position after changing cells ([#543](https://github.com/bpmn-io/dmn-js/issues/543))
* `FIX`: fix an error that was thrown when using the BACKSPACE key in literal expression editor in some situations ([#2095](https://github.com/camunda/camunda-modeler/issues/2095))
* `DEPS`: update to `dmn-js@11.0.2`

### Forms

* `FEAT`: allow setting the execution platform version for a form via the status bar ([#2323](https://github.com/camunda/camunda-modeler/issues/2323))
* `FEAT`: based on the selected execution platform version, show validation errors in case form components are not supported ([#2323](https://github.com/camunda/camunda-modeler/issues/2323))
* `DEPS`: update to `form-js@0.4.2` ([#2407](https://github.com/camunda/camunda-modeler/pull/2407))

## 4.9.0

### General

* `FEAT`: support Zeebe 1.1 / Camunda Cloud 1.1 ([#2319](https://github.com/camunda/camunda-modeler/issues/2319), [#2298](https://github.com/camunda/camunda-modeler/issues/2298), [#2297](https://github.com/camunda/camunda-modeler/issues/2297), [#2296](https://github.com/camunda/camunda-modeler/issues/2296))
* `FEAT`: improve status bar ([#2318](https://github.com/camunda/camunda-modeler/issues/2318), [#2303](https://github.com/camunda/camunda-modeler/issues/2303))
* `FEAT`: add basic what's new communication ([#2303](https://github.com/camunda/camunda-modeler/issues/2303))
* `FEAT`: remove ambiguous `+` button ([#2312](https://github.com/camunda/camunda-modeler/issues/2312), [#2293](https://github.com/camunda/camunda-modeler/issues/2293))
* `FEAT`: await loading of plug-in provided, injected styles ([`#2281`](https://github.com/camunda/camunda-modeler/pull/2281))
* `FIX`: correct opening of files in already running editor instance ([#2268](https://github.com/camunda/camunda-modeler/issues/2268))
* `CHORE`: migrate to GitHub actions ([#2245](https://github.com/camunda/camunda-modeler/issues/2245), [#2242](https://github.com/camunda/camunda-modeler/issues/2242))

### BPMN

* `FEAT`: support [bpmn-in-color](https://github.com/bpmn-miwg/bpmn-in-color)
* `FEAT`: support setting `variables` and `local` property via element templates independently ([#2334](https://github.com/camunda/camunda-modeler/issues/2334))
* `FIX`: support expressions in `bpmn:CallActivity#processId` field ([#2267](https://github.com/camunda/camunda-modeler/issues/2267))
* `FIX`: connect message flows to call activities ([#942](https://github.com/camunda/camunda-modeler/issues/942))
* `FIX`: correct Windows newlines being lost on paste ([#2280](https://github.com/camunda/camunda-modeler/issues/2280))
* `FIX`: report element template validation errors as warnings ([#2287](https://github.com/camunda/camunda-modeler/issues/2287))
* `FIX`: fallback to default properties panel layout ([#2255](https://github.com/camunda/camunda-modeler/issues/2255))
* `DEPS`: update to `bpmn-js@8.7.1`

### DMN

* `FEAT`: set focus on newly created row ([#2259](https://github.com/camunda/camunda-modeler/issues/2259))
* `FIX`: correct Windows newlines being lost on paste ([#2280](https://github.com/camunda/camunda-modeler/issues/2280))
* `DEPS`: update to `dmn-js@11.0.1`

### Forms

* `FEAT`: register Camunda Modeler for `.form` files on Windows ([#2292](https://github.com/camunda/camunda-modeler/issues/2292))
* `FIX`: open fallback editor if schema opening fails ([#2294](https://github.com/camunda/camunda-modeler/issues/2294))

## 4.8.1

* `FIX`: pass flags to client correctly ([#2257](https://github.com/camunda/camunda-modeler/pull/2257))

## 4.8.0

### General

* `FEAT`: enable Camunda Cloud BPMN tab ([#2210](https://github.com/camunda/camunda-modeler/issues/2210))
* `FEAT`: enable telemetry for engine version of deployments ([#2219](https://github.com/camunda/camunda-modeler/issues/2219))
* `FEAT`: enable telemetry for usage of BPMN service tasks ([#2218](https://github.com/camunda/camunda-modeler/issues/2218))
* `FEAT`: show error notification if update check triggered by user fails ([#2086](https://github.com/camunda/camunda-modeler/issues/2086))
* `FIX`: set minimum window size ([#2235](https://github.com/camunda/camunda-modeler/pull/2235))
* `FIX`: fix deployments of DMN to Camunda Platform ([#2241](https://github.com/camunda/camunda-modeler/issues/2241))
* `FIX`: fix error that appears when starting process instance ([#2249](https://github.com/camunda/camunda-modeler/issues/2249))
* `CHORE`: update to electron@12 ([#1926](https://github.com/camunda/camunda-modeler/issues/1926))
* `CHORE`: update to zeebe-node@1.0.0 ([#2169](https://github.com/camunda/camunda-modeler/issues/2169))

### BPMN

* `FEAT`: automatically scroll canvas when creating new elements ([#1249](https://github.com/camunda/camunda-modeler/issues/1249))
* `FIX`: copy root element references on replace ([#2185](https://github.com/camunda/camunda-modeler/issues/2185))
* `FIX`: do not override existing documentation ([#1682](https://github.com/camunda/camunda-modeler/issues/1682))
* `FIX`: reconnect message flows when collapsing participant ([#1651](https://github.com/camunda/camunda-modeler/issues/1651))
* `FIX`: don't change namespace prefixes of the xml namespace ([#2214](https://github.com/camunda/camunda-modeler/issues/2214))

## 4.7.0

### General

* `FEAT`: set `enable-duplicate-filtering` flag on deployments ([#2160](https://github.com/camunda/camunda-modeler/issues/2160))
* `FEAT`: allow deployments with multiple files ([#2131](https://github.com/camunda/camunda-modeler/issues/2131))
* `FEAT`: introduce status bar ([#2175](https://github.com/camunda/camunda-modeler/issues/2175))
* `FEAT`: introduce engine profile overlay ([#2187](https://github.com/camunda/camunda-modeler/issues/2187))
* `CHORE`: capture used Camunda Forms in telemetry events ([#2188](https://github.com/camunda/camunda-modeler/issues/2188))

### BPMN

* `FEAT`: support creating, opening, deploying and starting Zeebe BPMN diagrams ([#2029](https://github.com/camunda/camunda-modeler/issues/2029))
* `FEAT`: support non-default element templates for root elements ([#2121](https://github.com/camunda/camunda-modeler/issues/2121))
* `FEAT`: support BPMN Errors on external service tasks ([#2070](https://github.com/camunda/camunda-modeler/issues/2070))
* `FEAT`: introduce JSON Schema versioning via `$schema` property ([#2083](https://github.com/camunda/camunda-modeler/issues/2083))
* `FEAT`: validate element templates against JSON Schema ([#2159](https://github.com/camunda/camunda-modeler/issues/2159))
* `FEAT`: enable connection tool for text annotations ([#2042](https://github.com/camunda/camunda-modeler/issues/2042))
* `FIX`: support property panel plugins again ([#1992](https://github.com/camunda/camunda-modeler/issues/1992))
* `FIX`: consistently validate element templates in catalog ([#2110](https://github.com/camunda/camunda-modeler/issues/2110))
* `FIX`: improve error messages for element templates ([#2111](https://github.com/camunda/camunda-modeler/issues/2111))
* `FIX`: correctly display empty versions for element templates ([#2101](https://github.com/camunda/camunda-modeler/issues/2101))
* `FIX`: correctly display long variable names in the overview ([#2166](https://github.com/camunda/camunda-modeler/issues/2166))
* `CHORE`: disable Zeebe BPMN editor with flag ([#2171](https://github.com/camunda/camunda-modeler/pull/2171))
* `CHORE`: bump to `bpmn-js@8.3.0`
* `CHORE`: bump to `bpmn-js-properties-panel@0.42.0`

### DMN

* `CHORE`: bump to `dmn-js@10.1.0`

### Forms

* `FEAT`: add Forms editor ([#2149](https://github.com/camunda/camunda-modeler/issues/2149))
* `FEAT`: allow opening `.form` files ([#2108](https://github.com/camunda/camunda-modeler/issues/2108))
* `FEAT`: allow deploying Forms alongside BPMN diagrams ([#2100](https://github.com/camunda/camunda-modeler/issues/2100))

## 4.6.0

### General

* `FEAT`: offer `Check for Update` option in the menu ([#2010](https://github.com/camunda/camunda-modeler/issues/2010))
* `FEAT`: open fullscreen with Ctrl+Cmd+F on Mac ([#2050](https://github.com/camunda/camunda-modeler/issues/2050))
* `FIX`: correctly log filepath when logging a `write file` error ([#2079](https://github.com/camunda/camunda-modeler/pull/2079))
* `CHORE`: bump to `diagram-js@7.2.0`. Auxiliary mouse button events will now be passed as `element.*` mouse events to components (incl. components provided via plugins). You must filter your event listeners to prevent reactions to these events ([`1063f7c18`](https://github.com/bpmn-io/diagram-js/commit/1063f7c18474096d3d7c9e400ce82a1bf762a157)).

### BPMN

* `FEAT`: add `Participant-` prefix to respective `ID` and `Name` textInput labels to improve clarity ([#1738](https://github.com/camunda/camunda-modeler/issues/1738))
* `CHORE`: capture userTask formKey metrics on `diagram open` and `diagram deploy` events ([#2062](https://github.com/camunda/camunda-modeler/issues/2062))
* `FIX`: only catch DeploymentErrors and re-throw others when deploying a process or starting process instance fails ([#2078](https://github.com/camunda/camunda-modeler/issues/2078))
* `FIX`: only allow cancel boundary event on transaction subprocesses ([#2026](https://github.com/camunda/camunda-modeler/issues/2026))
* `CHORE`: bump to `bpmn-js@8.2.0`
* `CHORE`: bump to `bpmn-js-properties-panel@0.40.0`
* `CHORE`: bump to `@bpmn-io/extract-process-variables@0.4.0`

### DMN

* `FEAT`: add hand tool to DRD view ([#614](https://github.com/bpmn-io/dmn-js/pull/614))
* `FIX`: don't lose association when switching from DRD to DMN view ([#1874](https://github.com/camunda/camunda-modeler/issues/1874) and [#2052](https://github.com/camunda/camunda-modeler/issues/2052))
* `CHORE`: bump to `dmn-js@10.1.0-alpha.2`

## 4.5.0

### BPMN

* `FEAT`: support versioned element templates ([#1969](https://github.com/camunda/camunda-modeler/issues/1969))
* `FEAT`: support modeling `isCollection` marker for Data Object ([#381](https://github.com/bpmn-io/bpmn-js/issues/381))
* `FEAT`: support multi-instance pools ([#533](https://github.com/bpmn-io/bpmn-js/issues/533))
* `FEAT`: allow to replace Data Store Reference with Data Object Reference ([#1372](https://github.com/bpmn-io/bpmn-js/issues/1372))
* `FIX`: display local element templates in catalog ([#2012](https://github.com/camunda/camunda-modeler/issues/2012))
* `FIX`: allow to set external resource script value for I/O parameters ([#2007](https://github.com/camunda/camunda-modeler/issues/2007))
* `FIX`: escape element template properties ([#2031](https://github.com/camunda/camunda-modeler/issues/2031))
* `FIX`: rename Collapsed Pool to Empty Pool ([#2022](https://github.com/camunda/camunda-modeler/issues/2022))
* `FIX`: immediately activate tools when shortcut is pressed ([#664](https://github.com/camunda/camunda-modeler/issues/664), [#1229](https://github.com/camunda/camunda-modeler/issues/1229))
* `CHORE`: update to `bpmn-js@8.0.0`

### DMN

* `FEAT`: make decision table headers and the first column sticky ([#269](https://github.com/bpmn-io/dmn-js/issues/269))
* `FIX`: fix literal expression styles ([#2019](https://github.com/camunda/camunda-modeler/issues/2019))
* `CHORE`: update to `dmn-js@10.0.0`

### CMMN

* `FEAT`: set default value for `disable-cmmn`-flag to `true` ([#2036](https://github.com/camunda/camunda-modeler/issues/2036)); run with `--no-disable-cmmn` or edit your local [flags.json](https://docs.camunda.io/docs/components/modeler/desktop-modeler/flags/) to re-enable CMMN editor

## 4.4.0

### General

* `FEAT`: enable `Backspace` on MacOS for element removal ([#1989](https://github.com/camunda/camunda-modeler/issues/1989))
* `FEAT`: enable `SHIFT + click` for multi-selection ([#1964](https://github.com/camunda/camunda-modeler/issues/1964))
* `FIX`: correct switching between diagram and XML ([#1925](https://github.com/camunda/camunda-modeler/issues/1925))
* `CHORE`: capture deployment and process variables in telemetry events
* `CHORE`: bump to `bpmn-js@7.4.0`
* `CHORE`: bump to `dmn-js@9.4.0`
* `CHORE`: bump to `diagram-js@6.8.0`
* `CHORE`: bump to `bpmn-js-properties-panel@0.37.5`

### BPMN

* `FIX`: correct removal of element templates from events ([#1990](https://github.com/camunda/camunda-modeler/issues/1990))
* `FIX`: unlink incompatible element template during replace ([#1961](https://github.com/camunda/camunda-modeler/issues/1961))
* `FIX`: store variable events for conditional events in the correct property ([#836](https://github.com/camunda/camunda-modeler/issues/836))
* `FIX`: re-enable `entriesVisible` property of element templates ([#1975](https://github.com/camunda/camunda-modeler/issues/1975))
* `FIX`: correct label of start instance tool ([#1777](https://github.com/camunda/camunda-modeler/issues/1777))

### DMN

* `FEAT`: allow decision table name to take empty space
* `FEAT`: focus cell in newly added row ([#928](https://github.com/camunda/camunda-modeler/issues/928))
* `FIX`: render hit policy drop down in the correct location

## 4.3.0

### General

* `FEAT`: add modal menu to search and use element templates ([#1890](https://github.com/camunda/camunda-modeler/issues/1890))
* `FEAT`: introduce application, linking and unlinking logic of element templates ([#1889](https://github.com/camunda/camunda-modeler/issues/1889))
* `FIX`: prevent stopPropagation errors in iOS devices ([`0fbbbd1e`](https://github.com/bpmn-io/diagram-js/commit/0fbbbd1e439007d80c47158aa8774be3a592f936))
* `CHORE`: bump to `bpmn-js@7.3.1`
* `CHORE`: bump to `dmn-js@9.3.1`
* `CHORE`: bump to `diagram-js@6.7.1`
* `CHORE`: bump to `bpmn-js-properties-panel@0.37.1`

### BPMN

* `FEAT`: detect process variables in properties panel ([#348](https://github.com/bpmn-io/bpmn-js-properties-panel/issues/348))
* `FEAT`: improve input/output mapping GUI component in properties panel ([#349](https://github.com/bpmn-io/bpmn-js-properties-panel/issues/349))
* `FEAT`: add process variable overview for (sub) processes in properties panel ([#343](https://github.com/bpmn-io/bpmn-js-properties-panel/issues/343))
* `FEAT`: add process variable typeAhead functionality in properties panel ([#345](https://github.com/bpmn-io/bpmn-js-properties-panel/issues/345))
* `FEAT`: adjust element template view in properties panel ([#358](https://github.com/bpmn-io/bpmn-js-properties-panel/issues/358))
* `FEAT`: crop descriptions in properties panel ([#369](https://github.com/bpmn-io/bpmn-js-properties-panel/issues/369))
* `FIX`: allow incoming message flows to boundary message events ([#1919](https://github.com/camunda/camunda-modeler/issues/1919))

### DMN

* `FEAT`: improve intuition by recognising input and output columns ([#552](https://github.com/bpmn-io/dmn-js/issues/552))
* `FEAT`: move bpmn.io logo ([#573](https://github.com/bpmn-io/dmn-js/issues/573))
* `FIX`: clear clipboard after pasting ([#1246](https://github.com/camunda/camunda-modeler/issues/1246))
* `FIX`: handle undoing decision name direct editing ([#1912](https://github.com/camunda/camunda-modeler/issues/1912))
* `FIX`: handle undoing decision table components ([#1923](https://github.com/camunda/camunda-modeler/issues/1923))
* `FIX`: handle undoing deletion of decision elements ([#1921](https://github.com/camunda/camunda-modeler/issues/1921))
* `FIX`: handle undoing via keyboard ([#1922](https://github.com/camunda/camunda-modeler/issues/1922))
* `FIX`: save the size of resized text annotations in DRD ([#1941](https://github.com/camunda/camunda-modeler/issues/1941))
* `FIX`: fix broken keyboard shortcuts and menu entries for Undo & Redo in decision tables ([#1843](https://github.com/camunda/camunda-modeler/issues/1843))

## 4.2.0

### General

* `FEAT`: include CMMN diagramOpened event in usage-statistics ([#1887](https://github.com/camunda/camunda-modeler/issues/1887))
* `CHORE`: adjust colors to match CAMUNDA color scheme ([#1844](https://github.com/camunda/camunda-modeler/issues/1844))
* `FEAT`: allow plugins to get element templates from config ([#1893](https://github.com/camunda/camunda-modeler/pull/1893))
* `CHORE`: bump to `bpmn-js@7.3.0`
* `CHORE`: bump to `dmn-js@9.2.0`
* `CHORE`: bump to `diagram-js@6.7.0`

### BPMN

* `FIX`: disallow typed start events in sub processes ([#498](https://github.com/camunda/camunda-modeler/issues/498))

### DMN

* `FIX`: remove unnecessary click event cancel action ([#1907](https://github.com/camunda/camunda-modeler/issues/1907))
* `FEAT`: center the decision table resize hitbox ([#1906](https://github.com/camunda/camunda-modeler/issues/1906))
* `FEAT`: remove clause and rule menu entries  ([#1901](https://github.com/camunda/camunda-modeler/issues/1901))
* `FIX`: hide hit-policy input select on global mousedown event ([#1900](https://github.com/camunda/camunda-modeler/issues/1900))
* `FIX`: correct decision table allowed values layout ([#1895](https://github.com/camunda/camunda-modeler/issues/1895))
* `FIX`: complete direct editing on drill down in DRD ([#1892](https://github.com/camunda/camunda-modeler/issues/1892))
* `FIX`: correctly display DMN decision table dragging layout ([#1899](https://github.com/camunda/camunda-modeler/issues/1899))

## 4.1.1

### General

* `FIX`: remove _Create DMN Table_ from menu actions ([#1871](https://github.com/camunda/camunda-modeler/issues/1871))

### DMN

* `FIX`: correctly position cell header popup ([#1869](https://github.com/camunda/camunda-modeler/issues/1869))
* `FIX`: hide watermark for non-DRD modelers ([#1867](https://github.com/camunda/camunda-modeler/issues/1867))

## 4.1.0

### General

* `FEAT`: send ping and diagram creation events to E.T. telemetrics platform ([#1805](https://github.com/camunda/camunda-modeler/issues/1805))
* `FIX`: send correct source maps with crash reports ([#1813](https://github.com/camunda/camunda-modeler/issues/1831))
* `FIX`: ensure plugins are correctly sent to Sentry ([#1847](https://github.com/camunda/camunda-modeler/issues/1847))
* `FIX`: save workspace before quitting ([#1795](https://github.com/camunda/camunda-modeler/issues/1795))
* `FIX`: ensure space key is working to check / uncheck modal check boxes ([#1692](https://github.com/camunda/camunda-modeler/issues/1692))
* `FIX`: ensure menu is only initiated once ([#1816](https://github.com/camunda/camunda-modeler/issues/1816))

### BPMN

* `FEAT`: integrate promisified bpmn-js ([#1775](https://github.com/camunda/camunda-modeler/issues/1775))
* `CHORE`: bump to `bpmn-js@7.2.1`

### DMN

* `FEAT`: add DMN overview navigation ([#1767](https://github.com/camunda/camunda-modeler/issues/1767))
* `FEAT`: set default zoom scale when opening DMN overview ([#1848](https://github.com/camunda/camunda-modeler/issues/1848))
* `FEAT`: improve decision table layout ([#494](https://github.com/bpmn-io/dmn-js/issues/494))
* `FEAT`: improve literal expression layout ([#515](https://github.com/bpmn-io/dmn-js/issues/515))
* `FEAT`: add ability to resize table columns ([#500](https://github.com/bpmn-io/dmn-js/issues/500))
* `FIX`: allow association regardless of connection direction ([#1702](https://github.com/camunda/camunda-modeler/issues/1702))
* `FIX`: ensure select-all is working DMN properties panel ([#1685](https://github.com/camunda/camunda-modeler/issues/1685))
* `CHORE`: bump to `dmn-js@9.0.0`

## 4.0.0

* `CHORE`: bump to `bpmn-js@6.5.1`
* `CHORE`: bump to `cmmn-js@0.20.0`

## 4.0.0-alpha.3

#### General

* `FEAT`: Integrate error tracking ([#1796](https://github.com/camunda/camunda-modeler/pull/1796))
* `FEAT`: Update Camunda logo ([#1794](https://github.com/camunda/camunda-modeler/pull/1794))

## 4.0.0-alpha.2

#### General

* `FIX`: prevent loader from flickering ([#1743](https://github.com/camunda/camunda-modeler/pull/1743))
* `CHORE`: bump to `bpmn-js@6.5.0`
* `CHORE`: bump to `diagram-js@6.6.1`
* `CHORE`: bump to `dmn-js@8.3.0`
* `CHORE`: bump to `ids@1.0.0`
* `CHORE`: bump to `min-dash@3.5.2`

#### BPMN

* `FEAT`: prefer straight layout for sub-process connections ([#1309](https://github.com/bpmn-io/bpmn-js/pull/1309))

#### DMN

* `FEAT(drd)`: change layout of information requirements ([#492](https://github.com/bpmn-io/dmn-js/pull/492))
* `FEAT(drd)`: add auto-place feature ([#492](https://github.com/bpmn-io/dmn-js/pull/492))
* `FEAT(drd)`: connect from new shape to source on append ([#492](https://github.com/bpmn-io/dmn-js/pull/492))

## 3.7.3

#### General

* `CHORE`: bump to `dmn-js@7.5.1`

#### DMN

* `FIX`: changing decision ID via properties panel ([#1769](https://github.com/camunda/camunda-modeler/issues/1769))

## 3.7.2

#### General

* `CHORE`: bump to `bpmn-js@6.3.5`

#### BPMN

* `FIX`: correct accidental resizing of label target ([#1294](https://github.com/bpmn-io/bpmn-js/pull/1294))

## 4.0.0-alpha.1

#### General

* `FIX`: delayed validation in deployment tool after reopening the dialog ([#1741](https://github.com/camunda/camunda-modeler/issues/1741))

## 4.0.0-alpha.0

#### General

* `FEAT`: new loading indicator ([#1719](https://github.com/camunda/camunda-modeler/issues/1719))
* `FEAT`: completely overhauled UX of the deployment diagram ([#1709](https://github.com/camunda/camunda-modeler/issues/1709))
* `FEAT`: save and restore window size ([#576](https://github.com/camunda/camunda-modeler/issues/576))
* `FEAT`: apply native keyboard shortcuts in log panel ([#1380](https://github.com/camunda/camunda-modeler/issues/1380))
* `CHORE`: dialogs to return response instead of button ([`42d0ecc`](https://github.com/camunda/camunda-modeler/commit/42d0eccfae6143f472ec60b0280c7267b7d5a4e5))
* `CHORE`: remove watermark ([#1731](https://github.com/camunda/camunda-modeler/issues/1731))

#### DMN

* `FEAT`: support for opening DMN 1.2 and DMN 1.3 diagrams
* `FEAT`: migrate DMN 1.1 diagrams to DMN 1.3 on diagram open
* `FEAT`: migrate DMN diagrams to DMN 1.3 on export ([`7eb32a8`](https://github.com/camunda/camunda-modeler/commit/7eb32a80508c214c63257795b37dc430778871f3))
* `FEAT`: add resizing to DRD ([`3dd1265`](https://github.com/bpmn-io/dmn-js/commit/3dd12659bcc13abeb7e27cbcc9564a8171890abc))
* `FEAT`: improve DRD label editing ([#213](https://github.com/bpmn-io/dmn-js/issues/213))
* `FEAT`: set FEEL as default expression language ([#1710](https://github.com/camunda/camunda-modeler/issues/1710))
* `CHORE`: bump to `dmn-js@8.2.0`

### Breaking Changes

* DMN editor is migrated to DMN 1.3. Users will be able to open DMN 1.1 and DMN 1.2 diagrams, however exported diagrams will automatically be migrated to DMN 1.3. ([`7eb32a8`](https://github.com/camunda/camunda-modeler/commit/7eb32a80508c214c63257795b37dc430778871f3))
* This release is compatible with Camunda BPM versions 7.13.0, 7.12.4, 7.11.11, 7.10.17 and above.

## 3.7.1

#### General

* `FIX`: correctly export as image on Linux ([#1699](https://github.com/camunda/camunda-modeler/issues/1699))
* `FIX`: always paste as plain text to properties panels
* `CHORE`: make sure to daily check for updates if enabled ([`d2bf6a6`](https://github.com/camunda/camunda-modeler/commit/d2bf6a6fc147b73ecacaebdda7a334503d8c8928))

#### BPMN

* `FIX`: resize empty text annotations ([#1290](https://github.com/bpmn-io/bpmn-js/pull/1290))
* `FIX`: correctly move flows when adding lane ([#1715](https://github.com/camunda/camunda-modeler/issues/1715))
* `FIX`: restore semantic IDs for non flow nodes ([#1285](https://github.com/bpmn-io/bpmn-js/issues/1285))
* `FIX`: export BPMNDI in correct order ([#1326](https://github.com/camunda/camunda-modeler/issues/1326))
* `CHORE`: update to `bpmn-js@6.3.4`

#### DMN

* `FEAT(decision-table)`: add new rule on bottom rule \<enter> ([#345](https://github.com/bpmn-io/dmn-js/issues/345))
* `FEAT(drd)`: activate direct editing after text annotation create ([#185](https://github.com/bpmn-io/dmn-js/issues/185))
* `FIX`: update association's refs on element id change ([#397](https://github.com/bpmn-io/dmn-js/issues/397))
* `CHORE`:  update to `dmn-js@7.5.0`

## 3.7.0

#### General

* `FEAT`: disable deploy button if config is not valid ([`050fcdf`](https://github.com/camunda/camunda-modeler/commit/050fcdf364b4a9dc4aaad894c48b79d1c06e2050))
* `FEAT`: support Camunda Spring Boot starter per default ([#1610](https://github.com/camunda/camunda-modeler/issues/1610))
* `FEAT`: redeploy when running process with new config ([`b4f18fe`](https://github.com/camunda/camunda-modeler/commit/b4f18fe47d4c27ed7e4b8aaec789749c4c11bbbd))
* `FEAT`: improve look and responsiveness of modals ([#1681](https://github.com/camunda/camunda-modeler/issues/1681))
* `FEAT`: remove support for Linux 32bit platforms ([#1683](https://github.com/camunda/camunda-modeler/pull/1683))
* `FIX`: check for executable process before deploy and run ([#1671](https://github.com/camunda/camunda-modeler/issues/1671))
* `CHORE`: move modal styles to global ([#1691](https://github.com/camunda/camunda-modeler/pull/1691))
* `CHORE`: update to `electron@7.1.12`

#### BPMN

* `FEAT`: generate more generic IDs for new elements ([#1654](https://github.com/camunda/camunda-modeler/issues/1654))
* `FIX`: improve space tool ([#1368](https://github.com/camunda/camunda-modeler/issues/1368))
* `FIX`: correctly copy referenced root elements ([#1639](https://github.com/camunda/camunda-modeler/issues/1639))
* `FIX`: copy signal event variables ([#1684](https://github.com/camunda/camunda-modeler/issues/1684))
* `CHORE`: update to `bpmn-js@6.3.0`

#### DMN

* `FEAT`: add alignment buttons and snapping ([#1669](https://github.com/camunda/camunda-modeler/issues/1669))
* `FEAT`: add support for DMN Editor plugins ([#1550](https://github.com/camunda/camunda-modeler/pull/1550))
* `FIX`: do not display placeholder for input fields in table ([#1677](https://github.com/camunda/camunda-modeler/issues/1677))
* `FIX`: update XML correctly when changing id ([#1679](https://github.com/camunda/camunda-modeler/issues/1679))
* `FIX`: correct DMN Editor scrolling ([#1687](https://github.com/camunda/camunda-modeler/issues/1687))
* `CHORE`: update to `dmn-js@7.4.3`

## 3.6.0

#### General

* `FEAT`: add automatic update checks ([#1541](https://github.com/camunda/camunda-modeler/issues/1541))
* `FEAT`: allow to run BPMN processes directly from the app ([#1552](https://github.com/camunda/camunda-modeler/issues/1552))
* `FEAT`: make user data directory configurable ([#1625](https://github.com/camunda/camunda-modeler/issues/1625))
* `FIX`: make it possible to export huge diagrams as PNGs ([#1591](https://github.com/camunda/camunda-modeler/issues/1591))
* `FIX`: do not swallow warnings on editor open errors ([#1522](https://github.com/camunda/camunda-modeler/issues/1522))
* `FIX`: prevent illegal IDs from being entered in the properties panels ([#1623](https://github.com/camunda/camunda-modeler/issues/1623))
* `CHORE`: add clear primary / secondary actions for all dialogs
* `CHORE`: update to `Electron@7` as new app foundation ([#1448](https://github.com/camunda/camunda-modeler/issues/1448), [#1607](https://github.com/camunda/camunda-modeler/issues/1607))

#### BPMN

* `FEAT`: copy signals, escalations and errors ([#1049](https://github.com/camunda/camunda-modeler/issues/1049))
* `FEAT`: add horizontal and vertical resize handles
* `FEAT`: improve connection cropping
* `FIX`: correct creation of nested lanes ([#1617](https://github.com/camunda/camunda-modeler/issues/1617))
* `FIX`: disable re-layout behaviors on paste (paste as copied) ([#1611](https://github.com/camunda/camunda-modeler/issues/1611))
* `FIX`: do not open replace menu after multi-element create ([#1613](https://github.com/camunda/camunda-modeler/issues/1613))
* `FIX`: render colored `bpmn:Group` elements
* `FIX`: correct origin snapping on multi-element create ([#1612](https://github.com/camunda/camunda-modeler/issues/1612))
* `FIX`: properly reconnect message flows when collapsing participant
* `FIX`: keep non-duplicate outgoing connections when dropping on flow
* `FIX`: correct serialization of `DataAssociation#assignmet`
* `FIX`: allow `bpmn:Association` where `bpmn:DataAssociation` is allowed, too ([#1635](https://github.com/camunda/camunda-modeler/issues/1635))
* `CHORE`: update to `bpmn-js@6.2.1`

## 3.5.0

#### General

* `FEAT`: remember authentication details ([`eb35b078`](https://github.com/camunda/camunda-modeler/commit/eb35b07872b7a77936399532c99a7f485b99b012))
* `FEAT`: notarize MacOS distribution ([#1585](https://github.com/camunda/camunda-modeler/pull/1585))
* `FEAT`: trap focus and escape key in modal ([`4df45940`](https://github.com/camunda/camunda-modeler/commit/4df459409b893cc72e1287a04234511331e3adfe))
* `FEAT`: allow nodeIntegration to be enabled via feature toggle ([`c7f93c05`](https://github.com/camunda/camunda-modeler/commit/c7f93c05ad99dc400b2a259f88e0ad96de641aed))
* `FIX`: do not scroll clear/close controls ([`20b8dbfc`](https://github.com/camunda/camunda-modeler/commit/20b8dbfc2874238e7b5edc7256f63e3ad3282d9a))
* `CHORE`: prefix log messages with level ([`c741c41e`](https://github.com/camunda/camunda-modeler/commit/c741c41e3bbcfcf1176a783a9372006d16dcb688))
* `CHORE`: bump to `diagram-js@6.0.4`
* `CHORE`: bump to `bpmn-js@6.0.2`
* `CHORE`: bump to `dmn-js@7.2.1`

#### BPMN

* `FEAT`: connecting and re-connecting shapes is now possible in both directions ([#1230](https://github.com/bpmn-io/bpmn-js/pull/1230))
* `FIX`: render colored BPMN groups ([#1246](https://github.com/bpmn-io/bpmn-js/pull/1246))

### Breaking Changes

* `FEAT`: disable collapsing sub process ([`a2c008d0`](https://github.com/camunda/camunda-modeler/commit/a2c008d09effe200c857ec36a20889ae4dde598a))

#### DMN

* `FEAT(decision-table)`: preserve aggregation when COLLECT is selected again
* `FEAT(decision-table)`: allow aggreation to be cleared from dropdown ([#370](https://github.com/bpmn-io/dmn-js/issues/370), [#389](https://github.com/bpmn-io/dmn-js/issues/389))
* `FEAT(decision-table)`: use JUEL as the default input expression language ([#405](https://github.com/bpmn-io/dmn-js/issues/405))
* `FIX(decision-table)`: correctly handle value erasing ([#826](https://github.com/camunda/camunda-modeler/issues/826))
* `FIX(decision-table)`: correctly display simple mode edit control when cell selection changes ([#341](https://github.com/bpmn-io/dmn-js/issues/341))
* `FIX(decision-table)`: do not close input on user selection ([#421](https://github.com/bpmn-io/dmn-js/issues/421))
* `FIX(decision-table)`: do not navigate when clearing pre-defined hints ([#431](https://github.com/bpmn-io/dmn-js/issues/431))
* `FIX(decision-table)`: prevent context menu jump in larger tables
* `FIX(decision-table)`: do not close context on user selection

### Breaking Changes

* `FEAT(decision-table)`: only allow standardized hit policy values

## 3.4.1

* `FIX`: allow again to scroll DMN tables horizontally ([#1537](https://github.com/camunda/camunda-modeler/issues/1537))

## 3.4.0

#### General

* `FEAT`: add reusable notifications mechanism ([#1505](https://github.com/camunda/camunda-modeler/issues/1505))
* `FEAT`: allow access to workspace configurations for plugins and files ([#1425](https://github.com/camunda/camunda-modeler/issues/1425))
* `FIX`: complete direct editing on save operation ([#1473](https://github.com/camunda/camunda-modeler/issues/1473))
* `FIX`: correct autofocusing in modals ([#1489](https://github.com/camunda/camunda-modeler/pull/1489))
* `CHORE`: bump to `bpmn-js@5.1.0` / `diagram-js@5.1.0`

#### BPMN

* `FIX`: correct duplicated references in lanes ([#1504](https://github.com/camunda/camunda-modeler/issues/1504))
* `FIX`: keep sequence flow conditions after morphing source or target ([#180](https://github.com/camunda/camunda-modeler/issues/180))
* `FIX`: do not show preview if create operation is not allowed ([#1481](https://github.com/camunda/camunda-modeler/issues/1481))
* `FIX`: be able to paste elements on previously removed areas ([#1466](https://github.com/camunda/camunda-modeler/issues/1466))

#### Deployment

* `FEAT`: remember deployment details with diagram ([#1066](https://github.com/camunda/camunda-modeler/issues/1066))
* `FEAT`: display readable error message in log ([#1426](https://github.com/camunda/camunda-modeler/issues/1426))
* `FEAT`: derive default deployment name from the filename ([#1511](https://github.com/camunda/camunda-modeler/pull/1511))
* `FEAT`: deployment tool as a client extension ([#1488](https://github.com/camunda/camunda-modeler/issues/1488))

#### Plugins

* `FEAT`: add extension point for UI plugins ([#1490](https://github.com/camunda/camunda-modeler/issues/1490))
* Introduce several application events to hook into:
    * <tab.saved> ([#1498](https://github.com/camunda/camunda-modeler/pull/1498))
    * <tab.activeSheetChanged> ([`403afc`](https://github.com/camunda/camunda-modeler/commit/403afc920cf6c745816c3cd456baeb99830b25ed))
    * <app.activeTabChanged> ([`403afc`](https://github.com/camunda/camunda-modeler/commit/403afc920cf6c745816c3cd456baeb99830b25ed))
    * <bpmn.modeler.configure> ([#1499](https://github.com/camunda/camunda-modeler/issues/1499))
    * <bpmn.modeler.created> ([#1500](https://github.com/camunda/camunda-modeler/issues/1500))

## 3.3.5

* `FIX`: snap connections to shape center ([#1436](https://github.com/camunda/camunda-modeler/issues/1436))
* `FIX`: apply labels when using context pad ([#1502](https://github.com/camunda/camunda-modeler/issues/1502))
* `FIX`: do not copy extension elements with unknown type ([#1507](https://github.com/camunda/camunda-modeler/issues/1507))

## 3.3.4

* `FIX`: correct menu point visibility ([#1487](https://github.com/camunda/camunda-modeler/issues/1487))

## 3.3.3

* `FIX`: correct check whether plug-ins are enabled ([#1479](https://github.com/camunda/camunda-modeler/issues/1479))

## 3.3.2

* `FIX`: correct connection layout when dropping on sequence flows
* `CHORE`: bump to `bpmn-js@5.0.4`

## 3.3.1

* `FIX`: remove phantom snap lines showing on paste
* `CHORE`: bump to `bpmn-js@5.0.3` / `diagram-js@5.0.2`

## 3.3.0

#### General

* `FIX`: correct find shortcut not working ([#1450](https://github.com/camunda/camunda-modeler/issues/1450))
* `FIX`: restore paste shortcut not working in XML view ([#814](https://github.com/camunda/camunda-modeler/issues/814), [#868](https://github.com/camunda/camunda-modeler/issues/868))
* `CHORE`: disable node integration in client application ([#1453](https://github.com/camunda/camunda-modeler/pull/1453))

#### BPMN

* `FEAT`: add two-step copy and paste ([#1421](https://github.com/camunda/camunda-modeler/issues/1421))
* `FEAT`: make participants and expanded sub-processes draggable on borders and headers/labels only ([#238](https://github.com/camunda/camunda-modeler/issues/238))
* `FEAT`: improve navigation inside large participants / sub-processes ([#238](https://github.com/camunda/camunda-modeler/issues/238))
* `FEAT`: allow editing of `camunda:errorMessage` on `bpmn:Error` elements ([#1333](https://github.com/camunda/camunda-modeler/issues/1333))
* `FEAT`: add generic editor extension point ([#1434](https://github.com/camunda/camunda-modeler/pull/1434))
* `FEAT`: activate hand tool on `SPACE` ([#1475](https://github.com/camunda/camunda-modeler/pull/1475))
* `FIX`: allow participant to participant message flows to be copied ([#1413](https://github.com/camunda/camunda-modeler/issues/1413))
* `FIX`: do not update label positions when pasting ([#1325](https://github.com/camunda/camunda-modeler/issues/1325))
* `FIX`: keep allowed implementation details on copy and replace ([#681](https://github.com/camunda/camunda-modeler/issues/681), [#540](https://github.com/camunda/camunda-modeler/issues/540), [#647](https://github.com/camunda/camunda-modeler/issues/647), [#678](https://github.com/camunda/camunda-modeler/issues/678), [#538](https://github.com/camunda/camunda-modeler/issues/538), [#586](https://github.com/camunda/camunda-modeler/issues/586), [#537](https://github.com/camunda/camunda-modeler/issues/537), [#1464](https://github.com/camunda/camunda-modeler/issues/1464))
* `FIX`: allow editing of `camunda:InputOutput` in places supported by Camunda only ([#491](https://github.com/camunda/camunda-modeler/issues/491))
* `FIX`: make `camunda:failedJobsRetryTimeCycle` available consistently ([#1465](https://github.com/camunda/camunda-modeler/issues/1465))

#### Deploy

* `FEAT`: pre-fill deploy dialog with sensible defaults ([#1441](https://github.com/camunda/camunda-modeler/issues/1441))

## 3.2.3

* `FIX`: correct cursor being stuck in hover state ([#1383](https://github.com/camunda/camunda-modeler/issues/1383))
* `CHORE`: bump to `bpmn-js@4.0.4`

## 3.2.2

* `FIX`: make align-to-origin grid-aware
* `FIX`: allow deploy dialog to be closed without warnings ([#1405](https://github.com/camunda/camunda-modeler/issues/1405))

## 3.2.1

* `FIX`: prevent dropping on labels and groups in BPMN editor ([#1431](https://github.com/camunda/camunda-modeler/issues/1431))

## 3.2.0

#### General

* `FIX`: update properties panels to mitigate HTML injection vulnerabilities ([`1ed7caa2c`](https://github.com/camunda/camunda-modeler/commit/1ed7caa2ce3fe1a66b4b5786afbd63c1e54b9700), [blog post](https://bpmn.io/blog/posts/2019-html-injection-vulnerabilities-properties-panels-fixed.html))
* `CHORE`: validate that XML IDs for imported documents are valid [QNames](https://www.w3.org/2001/tag/doc/qnameids)

#### BPMN

* `FEAT`: add snap on resize ([#1290](https://github.com/camunda/camunda-modeler/issues/1290), [#609](https://github.com/camunda/camunda-modeler/issues/609), [#608](https://github.com/camunda/camunda-modeler/issues/608))
* `FEAT`: add ability to model `bpmn:Group` elements ([#464](https://github.com/camunda/camunda-modeler/issues/464))
* `FEAT`: add `bpmn:Subprocess` with start event included ([#1242](https://github.com/camunda/camunda-modeler/issues/1242))
* `FEAT`: make it easer to segment move ([#1197](https://github.com/camunda/camunda-modeler/issues/1197))
* `FEAT`: improve automatic label adjustment for boundary events ([#1206](https://github.com/camunda/camunda-modeler/issues/1206))
* `FEAT`: disallow multiple incoming connections on event-based gateway targets ([#637](https://github.com/camunda/camunda-modeler/issues/637))
* `FEAT`: improve layouting of boundary to activity loops ([#903](https://github.com/camunda/camunda-modeler/issues/903))
* `FEAT`: add grid snapping ([#1019](https://github.com/camunda/camunda-modeler/issues/1019))
* `FEAT`: add connection previews
* `FIX`: make message flow attachable to participants with lanes ([#1213](https://github.com/camunda/camunda-modeler/issues/1213))
* `FIX`: fix errors disappearing when adding colors ([#1342](https://github.com/camunda/camunda-modeler/issues/1342))
* `FIX`: correct name / id alignment in properties panel ([#1151](https://github.com/camunda/camunda-modeler/issues/1151))
* `FIX`: prevent unnecessary bendpoints ([#1204](https://github.com/camunda/camunda-modeler/issues/1204))
* `CHORE`: update to `bpmn-js@4.0.2`

#### CMMN

* `FEAT`: add connection previews
* `CHORE`: update to `cmmn-js@0.19.2`

## 3.1.2

* `FIX`: load local element templates ([#1379](https://github.com/camunda/camunda-modeler/pull/1379))
* `FIX`: apply default element templates only to new diagrams ([#1388](https://github.com/camunda/camunda-modeler/pull/1388))

## 3.1.1

* `FIX`: fix misleading log usage when `single-instance` flag is set to false ([#1363](https://github.com/camunda/camunda-modeler/issues/1363))

## 3.1.0

#### General

* `FIX`: restore keyboard shortcuts modal ([#1358](https://github.com/camunda/camunda-modeler/issues/1358))
* `FIX`: ignore `NODE_ENV` environment variable in production build ([#1352](https://github.com/camunda/camunda-modeler/issues/1352))
* `FIX`: keep changes when moving back and forth between unsafed tabs ([#1347](https://github.com/camunda/camunda-modeler/issues/1347))

#### BPMN

* `FEAT`: show `DataInput` / `DataOutput` labels ([#1324](https://github.com/camunda/camunda-modeler/issues/1324))
* `FEAT`: allow basic `DataInput` / `DataOutput` move
* `FIX`: prevent unnecessary dirty state without actual label update ([#858](https://github.com/camunda/camunda-modeler/issues/858))
* `CHORE`: update to `bpmn-js@3.3.1`

## 3.0.1

* `FIX`: fix desktop icons on Linux

## 3.0.0

#### General

* `CHORE`: update to `electron@3.1.7`
* `FIX`: show open file error dialog if tab couldn't be created ([#1320](https://github.com/camunda/camunda-modeler/pull/1320))
* `FIX`: fix DMN navigation ([#1321](https://github.com/camunda/camunda-modeler/pull/1321))
* `FIX`: update lastXML on xml prop change ([#1323](https://github.com/camunda/camunda-modeler/pull/1323))

#### BPMN

* `CHORE`: update to `bpmn-js@3.2.2`

## 3.0.0-beta.3

#### General

* `FEAT`: resize tab whenever app layout changes ([`8592eb4`](https://github.com/camunda/camunda-modeler/commit/8592eb479ba41fb3406416d91b84bd42d8439a4e))
* `FEAT`: mark file as unsaved if user cancels update ([#1188](https://github.com/camunda/camunda-modeler/issues/1188))
* `FEAT`: display error tab when editor fails ([#1214](https://github.com/camunda/camunda-modeler/issues/1214))
* `FEAT`: provide relevant context for tab errors ([#1176](https://github.com/camunda/camunda-modeler/issues/1176))
* `FEAT`: log mapped stack trace for errors ([`60393fe`](https://github.com/camunda/camunda-modeler/commit/60393fe0675359d304267601107e4c9e33cb53a6))
* `FEAT`: restore _Diagram opened with warnings_ hint ([#1177](https://github.com/camunda/camunda-modeler/issues/1177))
* `FEAT`: add simple way to restart editor without plug-ins ([#1253](https://github.com/camunda/camunda-modeler/issues/1253))
* `CHORE`: add license headers to all source files ([#1231](https://github.com/camunda/camunda-modeler/issues/1231))
* `CHORE`: add THIRD_PARTY_NOTICES ([#1233](https://github.com/camunda/camunda-modeler/issues/1233))
* `FIX`: only show plug-ins menu if plug-ins are registered ([#1239](https://github.com/camunda/camunda-modeler/issues/1239))
* `FIX`: restore menu state backwards compatibility ([#1193](https://github.com/camunda/camunda-modeler/issues/1193))
* `FIX`: disable _reopen last tab_ menu button when there is no last tab ([#1173](https://github.com/camunda/camunda-modeler/issues/1173))
* `FIX`: disable _save as_ menu button for empty tab ([#1282](https://github.com/camunda/camunda-modeler/issues/1282))
* `FIX`: import xml to editor only when it is changed ([`3f9cdaf`](https://github.com/camunda/camunda-modeler/commit/3f9cdafaad85eb4907c8cbe03a5230ffc4960456), [#1298](https://github.com/camunda/camunda-modeler/issues/1298))
* `FIX`: allow well-known files to be dropped ([`46ae9b1`](https://github.com/camunda/camunda-modeler/commit/46ae9b1bf44b52c92f3a7cd8f2cf875593aca51c))
* `FIX`: restore empty file dialog ([#1301](https://github.com/camunda/camunda-modeler/issues/1301))
* `FIX`: correct undo/redo behavior ([#1218](https://github.com/camunda/camunda-modeler/issues/1218))
* `FIX`: disable plugin menu item when function returns falsy value ([#1311](https://github.com/camunda/camunda-modeler/pull/1311))

#### BPMN

* `CHORE`: update to `bpmn-js@3.2.2`
* `FIX`: gracefully handle missing waypoints ([`45486f2`](https://github.com/bpmn-io/bpmn-js/commit/45486f2afe7f42fcac31be9ca477a7c94babe7d8))
* `FIX`: restore error dialog for broken diagram ([#1192](https://github.com/camunda/camunda-modeler/issues/1192))
* `FIX`: replace namespace util to not parse diagram twice ([`bdee98e`](https://github.com/camunda/camunda-modeler/commit/bdee98e1b34fa6088ce71d6d9ebf4b339cb812cc))

#### DMN

* `FEAT`: show input and output label first in editors ([#346](https://github.com/bpmn-io/dmn-js/issues/346))
* `CHORE`: update to `dmn-js@6.3.2`
* `FIX`: set dirty state correctly when view is changed
* `FIX`: properly destroy individual viewers on dmn-js destruction ([#392](https://github.com/bpmn-io/dmn-js/pull/392))
* `FIX`: change active view when sheets change ([#1310](https://github.com/camunda/camunda-modeler/pull/1310))

## 3.0.0-beta.2

#### General

* `CHORE`: restore improved image resolution, supposedly shipped with `v3.0.0-0` already ([#486](https://github.com/camunda/camunda-modeler/issues/486))
* `FIX`: set align to origin offset to saner default
* `FIX`: ensure new diagrams contain unique ids for process, case and decision elements

## 3.0.0-beta.1

#### General

* `FIX`: handle unrecognized, non-file arguments passed to application ([#1237](https://github.com/camunda/camunda-modeler/issues/1237))

## 3.0.0-beta.0

#### General

* `FEAT`: add feature toggles ([#1159](https://github.com/camunda/camunda-modeler/issues/1159))
* `FEAT`: add BPMN only mode ([#872](https://github.com/camunda/camunda-modeler/issues/872))
* `FEAT`: rework file dropping
* `FEAT`: improve logging across the application
* `FEAT`: allow disabling plug-ins via flag ([`4b365482`](https://github.com/camunda/camunda-modeler/commit/4b3654825d033035e588e33927ceee4ce089af44))
* `FEAT`: align diagrams to `(0,0)` on save to prevent negative coordinates ([#982](https://github.com/camunda/camunda-modeler/issues/982), [#1183](https://github.com/camunda/camunda-modeler/issues/1183))
* `FEAT`: drop diagram origin cross ([#1096](https://github.com/camunda/camunda-modeler/issues/1096))
* `FEAT`: unify search paths for plug-ins and element templates ([#597](https://github.com/camunda/camunda-modeler/issues/597))
* `FEAT`: show full path to diagram as tab title ([#1187](https://github.com/camunda/camunda-modeler/issues/1187))
* `FEAT`: make application logs available on file system ([#1156](https://github.com/camunda/camunda-modeler/issues/1156))
* `CHORE`: update to `electron@3.1.3`
* `CHORE`: update to `bpmn-js@3.2.0`
* `FIX`: correct shortcuts shown in overlay ([#1039](https://github.com/camunda/camunda-modeler/issues/1039))
* `FIX`: properly handle file-drop in XML view ([#571](https://github.com/camunda/camunda-modeler/issues/571))
* `FIX`: don't throw error when dragging file over diagram tabs ([#1120](https://github.com/camunda/camunda-modeler/issues/1120))
* `FIX`: prevent jumping when resizing properties/log panels ([`f68e6764`](https://github.com/camunda/camunda-modeler/commit/f68e67643f6fa0cba2ac69f7a832868485b0fc68))
* `FIX`: re-open + focus docked app on file open (MacOS) ([`eff83531`](https://github.com/camunda/camunda-modeler/commit/eff83531b0d5a7d2735f3f4987048d47743e1f9d))
* `FIX`: prevent external file changed dialog from opening twice on Windows / Linux ([#1118](https://github.com/camunda/camunda-modeler/issues/1118))

#### BPMN

* `FEAT`: set `isHorizontal` to `bpmndi:Shape` elements ([#1096](https://github.com/camunda/camunda-modeler/issues/1096))
* `FIX`: mark diagram as dirty after `activiti` to `camunda` namespace conversion ([#403](https://github.com/camunda/camunda-modeler/issues/403))

#### Deploy Dialog

* `FEAT`: set `deployment-source` to `Camunda Modeler` ([#1153](https://github.com/camunda/camunda-modeler/issues/1153))

#### Plug-ins

* `FEAT`: add ability to reference local assets via logical paths ([`dcf2bc0b`](https://github.com/camunda/camunda-modeler/commit/dcf2bc0bbc2450608992d343d32b2304531c3a80))
* `FEAT`: recognize plug-ins in `{basePath}/resources/plugins` ([#597](https://github.com/camunda/camunda-modeler/issues/597))
* `CHORE`: gracefully handle plugin load failures ([#1180](https://github.com/camunda/camunda-modeler/issues/1180))
* `CHORE`: enforce unique names ([#1180](https://github.com/camunda/camunda-modeler/issues/1180))
* `CHORE`: log loading and activation ([#1180](https://github.com/camunda/camunda-modeler/issues/1180))
* `CHORE`: improve plugin error handling in various places ([`d916d22f`](https://github.com/camunda/camunda-modeler/commit/d916d22f6a9663d0302e9f2cb6a05521800a1942), [`420cf831`](https://github.com/camunda/camunda-modeler/commit/420cf83137e337b2f42db2acc9ac07d5fc80a0d4), [`39e3c2eb`](https://github.com/camunda/camunda-modeler/commit/39e3c2eb0d47cbebc07c431e182e801518fb14da))
* `CHORE`: deprecate global plug-in helpers in favor of logical paths ([`1de7af5a`](https://github.com/camunda/camunda-modeler/commit/1de7af5a89704715648ec2f3728a2ac4da660661))
* `FIX`: give plug-ins stored in `{userData}` access to local assets ([#1135](https://github.com/camunda/camunda-modeler/issues/1135))


### Breaking Changes

* The global plug-in helper `getPluginPaths()` did not work reliably and got deprecated. Use logical paths of the form `app-plugins://{pluginName}/{pathToResource}` to reference static plug-in assets ([`1de7af5a`](https://github.com/camunda/camunda-modeler/commit/1de7af5a89704715648ec2f3728a2ac4da660661)).
* The global plug-in helper `getModelerPath()` was removed without replacement ([`1de7af5a`](https://github.com/camunda/camunda-modeler/commit/1de7af5a89704715648ec2f3728a2ac4da660661)).
* Rewriting the modeler changed most CSS selectors outside the actual diagram editors / properties panels. This may break plug-ins that monkey patch the application styles.
* To improve compatibility with external tools, we now prevent negative coordinates by aligning to `(0,0)` on diagram save. This results in slightly more noise in actual file changes ([#1096](https://github.com/camunda/camunda-modeler/issues/1096)).



## 3.0.0-0

_This is a pre-release of the app ported to an entirely new architecture._

#### General

* `FEAT`: add ability for users to give feedback via the Help menu ([#1094](https://github.com/camunda/camunda-modeler/issues/1094))
* `FEAT`: improve resolution of exported images ([#486](https://github.com/camunda/camunda-modeler/issues/486))
* `CHORE`: rewrite client app in ReactJS ([#866](https://github.com/camunda/camunda-modeler/issues/866))
* `CHORE`: rewrite back-end for better separation of concerns and extensibility ([#866](https://github.com/camunda/camunda-modeler/issues/866))
* `CHORE`: rework back-end to client communication ([#866](https://github.com/camunda/camunda-modeler/issues/866))
* `CHORE`: update to `electron@3.0.14`
* `FIX`: do not restrict height of properties panel content ([#283](https://github.com/bpmn-io/bpmn-js-properties-panel/pull/283), [#62](https://github.com/bpmn-io/cmmn-js-properties-panel/pull/62), [#6](https://github.com/bpmn-io/dmn-js-properties-panel/pull/6))

#### Deploy Dialog

* `FEAT`: add ability to use authentication ([#1063](https://github.com/camunda/camunda-modeler/pull/1063), [#742](https://github.com/camunda/camunda-modeler/pull/742))
* `FEAT`: remember last deployed endpoint URL ([#1041](https://github.com/camunda/camunda-modeler/pull/1041))
* `FEAT`: improve error handling ([#838](https://github.com/camunda/camunda-modeler/issues/838), [#846](https://github.com/camunda/camunda-modeler/issues/846))
* `FEAT`: deploy only changed resources per default ([#744](https://github.com/camunda/camunda-modeler/issues/744))
* `FIX`: disable editor shortcuts while modal is active ([#929](https://github.com/camunda/camunda-modeler/issues/929))

#### BPMN

* `FEAT`: add hints to returned Java types in properties panel ([#286](https://github.com/bpmn-io/bpmn-js-properties-panel/pull/286))
* `FEAT`: show target variable name instead of index in properties panel ([#287](https://github.com/bpmn-io/bpmn-js-properties-panel/pull/287))
* `CHORE`: update to `bpmn-js@3.1.0`
* `FIX`: render labels always on top ([#1050](https://github.com/camunda/camunda-modeler/issues/1050))

#### DMN

* `FEAT`: add ability to navigate all decision elements using tabs
* `CHORE`: update to `dmn-js@6.2.0`
* `FIX`: correct dirty state indicator

#### CMMN

* `CHORE`: update to `cmmn-js@0.17.0`

## 2.2.4

#### BPMN

* `FIX`: include `camunda:calledElementVersionTag` ([#1074](https://github.com/camunda/camunda-modeler/issues/1074))

## 2.2.3

#### BPMN

* `FIX`: do not join incoming/outgoing flows other than sequence flows on element deletion ([#1033](https://github.com/camunda/camunda-modeler/issues/1033))

## 2.2.2

* `CHORE`: drop unused dependency

## 2.2.1

* `FIX`: correct `camunda:isStartableInTasklist` default value

## 2.2.0

#### General

* `FEAT`: support moving elements via keyboard arrows on all diagram editors ([`a2b5bf07`](https://github.com/camunda/camunda-modeler/commit/a2b5bf079574a90bd1377150c7c39aab181261a6))
* `FEAT`: add accessible context-pad and popup-menu to all remaining diagram editors (DRD, CMMN)
* `CHORE`: update to `cmmn-js@0.16.0`
* `CHORE`: update to `dmn-js@6.0.0`
* `FIX`: correct properties panel scrolling with many items

#### BPMN

* `FEAT`: add editing support for `camunda:isStartableInTasklist` ([#843](https://github.com/camunda/camunda-modeler/issues/843))

#### DMN

* `FEAT`: support moving canvas via keyboard arrows in DRD editor ([#1016](https://github.com/camunda/camunda-modeler/issues/1016))
* `FEAT`: add diagram origin cross in DRD editor ([`7dceaf5f9`](https://github.com/camunda/camunda-modeler/commit/7dceaf5f9b764426fa1c647bc7e6b4ffe9148fbb))

## 2.1.2

* `CHORE`: update dependencies

## 2.1.1

* `FIX`: fix move canvas key binding in BPMN editor

## 2.1.0

#### General

* `FEAT`: moving the canvas using keyboard arrows now requires the `Ctrl/Cmd` modifier
* `FIX`: correctly detect file type when opening file ([#944](https://github.com/camunda/camunda-modeler/issues/944))
* `CHORE`: bump to `electron@3.0.0`

#### BPMN

* `FEAT`: add moddle extensions as plugins to bpmn-js ([#949](https://github.com/camunda/camunda-modeler/pull/949))
* `FEAT`: display group names ([#844](https://github.com/bpmn-io/bpmn-js/issues/844))
* `FEAT`: add ability to move selection with keyboard arrows ([#376](https://github.com/bpmn-io/bpmn-js/issues/376))
* `FEAT`: improve `EventBasedGateway` context pad tooltips ([#917](https://github.com/camunda/camunda-modeler/issues/917))
* `FEAT`: improve modeling behavior after `EventBasedGateway` ([#784](https://github.com/camunda/camunda-modeler/issues/784))
* `CHORE`: update to `bpmn-js@3`

#### DMN

* `CHORE`: update to `dmn-js@5.2.0`

#### CMMN

* `CHORE`: update to `cmmn-js@0.15.2`

## 2.0.3

_Republish of `v2.0.2` with fixed distribution_.

## 2.0.2

* `FIX`: fix native copy and paste in DMN decision tables on MacOS ([#758](https://github.com/camunda/camunda-modeler/issues/758))

## 2.0.1

* `FIX`: correct MacOS app icon size ([#901](https://github.com/camunda/camunda-modeler/issues/901))

## 2.0.0

* `CHORE`: update to `bpmn-js-properties-panel@0.26.2`

## 2.0.0-6

_This is a pre-release_.

* `CHORE`: update to `bpmn-js@2.5.1`

## 2.0.0-5

_This is a pre-release_.

* `CHORE`: drop unused dependency

## 2.0.0-4

_This is a pre-release_.

* `CHORE`: bump `electron` version

## 2.0.0-3

_This is a pre-release_.

#### General

* `CHORE`: drop Windows installer, as it is currently broken (cf. [#867](https://github.com/camunda/camunda-modeler/issues/867))

#### BPMN

* `FEAT`: snap `bpmn:Event` to center when creating message flows ([#887](https://github.com/camunda/camunda-modeler/issues/887))
* `FIX`: prevent error dragging label onto `bpmn:MessageFlow` ([#888](https://github.com/camunda/camunda-modeler/issues/888))
* `FIX`: round coordinates when dragging elements ([#886](https://github.com/camunda/camunda-modeler/issues/886))


## 2.0.0-2

_This is a pre-release_.

* `FIX`: properly reflect decision id changes in decision table and literal expression editors

## 2.0.0-1

_This is a pre-release_.

* `FEAT`: add DMN properties panel, avaliable for all DMN editors ([#847](https://github.com/camunda/camunda-modeler/issues/847))
* `FEAT`: add ability to edit `camunda:historyTimeToLive` on `dmn:Decision` elements ([#581](https://github.com/camunda/camunda-modeler/issues/581))
* `FEAT`: add ability to edit `camunda:versionTag` on `dmn:Decision` elements ([#802](https://github.com/camunda/camunda-modeler/issues/802))
* `CHORE`: drop `dmn:Definitions` `name` and `id` editing from DRD editor; you may edit these properties via the DMN properties panel ([`653eb607`](https://github.com/camunda/camunda-modeler/commits/653eb607183c6cf0457b8023a2d61cf8343da7fb))

## 2.0.0-0

_This is a pre-release_.

* `FEAT`: improve minimap, round two
* `FEAT`: support boundary event to activity loops ([#776](https://github.com/camunda/camunda-modeler/issues/776))
* `FEAT`: support activity to activity loops
* `FEAT`: provide Windows installer and MacOS DMG distribution ([#787](https://github.com/camunda/camunda-modeler/issues/787))
* `FEAT`: sign executables on Windows and MacOS ([#787](https://github.com/camunda/camunda-modeler/issues/787))
* `CHORE`: update to `bpmn-js@2.4.0`
* `CHORE`: update to `cmmn-js@0.15.0`
* `CHORE`: update to `diagram-js-minimap@1.2.2`
* `CHORE`: drop in-app Windows file association behavior in favor of external support script ([`a07b693a`](https://github.com/camunda/camunda-modeler/commits/a07b693a9648715af0410cc13f5c58dcbea2f3df))
* `FIX`: correct minimap collapse icon
* `FIX`: correct app icons ([#503](https://github.com/camunda/camunda-modeler/issues/503))
* `FIX`: prevent creation of duplicate flows in BPMN editor ([#777](https://github.com/camunda/camunda-modeler/issues/777))

## 1.16.2

* `FIX`: correctly update editor actions on direct editing ([#790](https://github.com/camunda/camunda-modeler/issues/790), [#834](https://github.com/camunda/camunda-modeler/issues/834))
* `FIX`: use `Arial` as default font when exporting SVG ([#840](https://github.com/camunda/camunda-modeler/issues/840))
* `CHORE`: update to `dmn-js@5.1.0`
* `CHORE`: update to `bpmn-js@2.3.1`

## 1.16.1

* `FIX`: correct bpmn-js version used in lock file
* `CHORE`: update to `bpmn-js@2.2.1`

## 1.16.0

* `FEAT`: show loader on application startup
* `FEAT`: resize text annotation when editing via properties panel ([#631](https://github.com/camunda/camunda-modeler/issues/631))
* `FIX`: correct error message on import error ([#821](https://github.com/camunda/camunda-modeler/issues/821))
* `FIX`: create/update labels when updating element name via properties panel ([#824](https://github.com/camunda/camunda-modeler/issues/824))
* `FIX`: correct target attribute in signal payload not being removed from BPMN 2.0 XML ([#818](https://github.com/camunda/camunda-modeler/issues/818))
* `CHORE`: update to `bpmn-js@2.2.0`
* `CHORE`: update to `diagram-js-minimap@1`

## 1.15.1

* `CHORE`: make dialogs actual modal windows ([#815](https://github.com/camunda/camunda-modeler/pull/815))

## 1.15.0

* `FEAT`: allow data stores to be modeled between participants ([#183](https://github.com/camunda/camunda-modeler/issues/183))
* `FEAT`: allow deletion of external labels, clearing text ([#243](https://github.com/camunda/camunda-modeler/issues/243))
* `FEAT`: speed up BPMN diagram import by only rendering non-empty labels
* `FEAT`: show loader when opening huge diagrams ([#704](https://github.com/camunda/camunda-modeler/issues/704))
* `FEAT`: export image using native type chooser ([#171](https://github.com/camunda/camunda-modeler/issues/171))
* `CHORE`: improve text rendering in BPMN diagrams
* `FIX`: correct BPMN editor align button tooltip ([#590](https://github.com/camunda/camunda-modeler/issues/590))
* `FIX`: make `cycle` option for BPMN intermediate timer events available again ([#792](https://github.com/camunda/camunda-modeler/issues/792))
* `FIX`: correct edit menu on direct editing activation ([#708](https://github.com/camunda/camunda-modeler/issues/708))
* `FIX`: prevent BPMN element deletion when pressing `DEL` in BPMN properties panel ([#680](https://github.com/camunda/camunda-modeler/issues/680))
* `CHORE`: update to `Electron@2`
* `CHORE`: update to `bpmn-js@2.1.0`
* `CHORE`: update to `bpmn-js-properties-panel@0.25.1`

## 1.14.0

* `FEAT`: add ability to create a new diagram when opening an empty file ([#636](https://github.com/camunda/camunda-modeler/issues/636))
* `FEAT`: improve compatibility with Signavio BPMN 2.0 exports ([#732](https://github.com/camunda/camunda-modeler/issues/732))
* `FIX`: correct context menu positioning in decision table editor

## ...

Check `git log` for earlier history.
