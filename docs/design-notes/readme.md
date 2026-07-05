# Code architecture documentation

This is a collection of design-oriented documentation for different parts of the WinUI codebase. It is an
ongoing effort, so expect changes to both content and format over time.

Docs here fall into three broad kinds:

- **Architecture & concepts** - living documents describing how a subsystem works.
- **Control & feature overviews** - higher-level tours of a specific control or feature area.
- **API & feature specs** - point-in-time proposal/spec documents captured when a feature was designed. These are
  *not* maintained as living docs and may not exactly match the current implementation.

> Tip: If you add a doc to this folder, add a link to it below so it does not become orphaned.

## Start here

- [Journey of a control](./control-overview.md) - a vertical slice of what makes up a WinUI control.
- [Guide to WinUI codebase pointers](./pointers.md) - where to find things in the code.
- [Dxaml vs Core layers / Peer objects](./dxamlvscore.md) - the two-layer object model and how to transition between them.
- [Startup path for a WinUI application](./startup-overview.md)
- [XAML Rendering Architecture](./rendering.md) - how the rendering engine integrates with the system compositor.

## Architecture & concepts

### Compiler, codegen & type system

- [XAML Compiler Development and Architecture](./xamlcompiler.md)
- [Codegen](./codegen.md)
- [A/B Forward Compatibility - XAML Parser and XamlCompiler](./abforward-xamlparser-xamlcompiler.md)
- [WinUI3 APIs and FastAbi](./fastabi.md)
- [List of Lifted WinUI XAML Types](./lifted-xaml-types.md)
- [Consolidating the Microsoft.UI namespace to one package](./consolidate-microsoft-ui-namespace.md)
- [DependencyObject](./dependency-object.md)
- [Lightweight Bindings](./lightweight-bindings.md)

### Object lifetime, threading & scheduling

- [XAML/C# Object Lifetime Design](./xaml-object-lifetime.md) ([links](./xaml-object-lifetime-links.md))
- [UI Thread Ticking](./ui-thread-ticking.md)
- [XAML scheduling](./scheduling.md)
- [Reentrancy](./reentrancy.md)
- [XAML Shutdown](./xaml-shutdown.md)
- [Loading / Loaded / Unloaded events](./loading-loaded-unloaded-events.md)

### Rendering, layout & visuals

- [XAML's usage of surfaces](./surfaces-overview.md)
- [Layout manager overview](./Layout-overview.md)
- [XAML Animations](./animation.md)
- [XAML Imaging](./imaging.md)
- [Mica / Desktop Acrylic](./mica-desktop-acrylic.md)
- [Lifted XAML and OneCoreTransforms](./OneCoreTransforms.md)
- [Direct Manipulation Integration](./direct-manipulation.md)
- [XAML Popups](./popup.md) and [Popup system backdrop](./popup-system-backdrop.md)
- [XAML RTL](./rtl.md) and [IXP RTL Layout (end to end)](./rtlEndToEnd.md)

### Resources, styles & theming

- [Resources - Functional and Dev Design](./resources.md)
- [XAML Styles](./styles.md)
- [XAML Style Guide](./xaml-styling-guide.md)
- [Custom MRT ResourceManager for apps](./custom-mrt-resourcemanager.md)

### Input, focus, text & accessibility

- [XAML Input](./input.md)
- [Focus in WinUI 3](./focus.md)
- [Inking in XAML](./ink.md)
- [TSF in WinUI3](./tsf-in-winui3.md)
- [Read-Only Text Controls Architecture](./text-controls.md)
- [UIA (accessibility)](./Uia.md)
- [AccessKeyManager.EnterDisplayMode](./enter-display-mode.md)
- [ContextFlyout Property](./context-flyout.md)

### App model, windowing & hosting

- [XAML App Model](./app-model.md)
- [XAML Window](./xaml-window.md)
- [Custom Title Bar](./customtitlebar.md)
- [Unpackaged Windows App SDK apps](./unpackaged-apps.md)
- [XamlBehaviors](./xamlbehaviors.md) - deprecated features still being phased out.

### Diagnostics & debugging

- [DebugSettings](./debug-settings.md)
- [Improving Diagnosability of Missing XAML Resources](./xaml-resource-lookup-failure-tracing.md)
- [Inspecting a WinUI Desktop app](./desktop-app-walkthrough.md)

## Control & feature overviews

- [ItemsRepeater overview](./ItemsRepeater-overview.md)
- [ItemsView / ItemContainer overviews](./ItemsView-ItemContainer-overview.md)
- [ListView / GridView overview](./ListView-GridView-overview.md)
- [ScrollView / ScrollPresenter / IScrollController overviews](./ScrollView-overview.md)
- [ScrollViewer overview](./ScrollViewer-overview.md)

## API & feature specs

> These are point-in-time design specs and may not reflect the current implementation.

- [AnnotatedScrollBar API spec](./annotatedscrollbar_spec.md)
- [Custom title bar for WinUI 3](./customtitlebar-spec.md)
- [DebugSettings Layout Cycle Debugging API spec](./debug-settings-layoutCycle-spec.md)
- [Application.DispatcherShutdownMode](./dispatchershutdownmode-spec.md)
- [InfoBadge control](./InfoBadge-spec.md)
- [ItemContainer (functional spec)](./itemcontainer-functional-spec.md)
- [ItemCollectionTransitionProvider API spec](./ItemCollectionTransitionProvider-spec.md)
- [ItemsView control API spec](./ItemsView_spec.md)
- [LinedFlowLayout API spec](./LinedFlowLayout_spec.md)
- [Layout updates for LinedFlowLayout](./layout-updates-for-lfl.md)
- [Map Control API spec](./mapControl-spec.md)
- [ScrollPresenter & IScrollController API spec](./ScrollPresenter-spec.md)
- [ScrollView API spec](./ScrollView-spec.md)
- [Symbol Enum](./symbol-enum-spec.md)
- [Tab Tear-Out spec](./TabTearOut-spec.md) and [Tab Tear-Out API spec](./TabTearOut-API-spec.md)
- [TreeView.SelectionChanged API spec](./TreeView-SelectionChanged-spec.md)
- [WindowsXamlManager Shutdown Improvements spec](./windowsxamlmanager-shutdownimprovements-spec.md)
- [ContentDialogPlacement.UnconstrainedPopup](./unconstrained-popup.md)
- [WebView2 Support for Custom Environment/Options](./wv2-custom-environment-spec.md)

## Subsystems

### XAML Islands

See the [XAML Islands overview](./xaml-islands/README.md) for the full index. Key docs:

- [XamlIsland type](./xaml-islands/xaml-island-type.md)
- [XamlIsland implementation](./xaml-islands/xaml-island-impl.md)
- [XAML Island and Multi-Window Plans/Design](./xaml-islands/xaml-islands.md)
- [DesktopWindowXamlSource](./xaml-islands/desktopwindowxamlsource.md)
- [Windowless XamlIslands](./xaml-islands/windowless-xaml-islands.md)
- [XAML Island Focus Navigation](./xaml-islands/xaml-island-focus-navigation.md)
- [XAML Islands and DispatcherQueue](./xaml-islands/xaml-islands-and-dispatcherqueue.md)
- [Can XAML host a ContentIsland?](./xaml-islands/xaml-hosting-islands.md)
- [React Native Windows and XAML](./xaml-islands/react-native-windows.md)

### SelectorBar / Segmented

- [SelectorBar functional spec](./SelectorBar/selectorBar-functional-spec.md)
- [Segmented functional spec](./SelectorBar/segmented-functional-spec.md)
- [Segmented dev spec](./SelectorBar/segmented-dev-spec.md)

### TitleBar

- [TitleBar functional spec](./TitleBar/titlebar-functional-spec.md)
- [TitleBar dev spec](./TitleBar/titleBar-dev-spec.md)