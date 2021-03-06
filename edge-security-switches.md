# Introduction
This file details all the Microsoft Edge switches that have been modified in my [security guide](https://cutechri.xyz). Not all of them have an explanation, this section serves mostly as a list of all the changes, in case the commandline is unreadable.

## Batch file

Here is the code of the batch file I mentioned in my guide. Simply copy and paste it.

```
@echo off
start "" "%cd%\msedge.exe" --disable-breakpad --disable-domain-reliability --disable-external-intent-requests --disable-file-system --extension-content-verification=enforce_strict --extensions-install-verification=enforce  --no-pings --process-per-site --site-per-process --enable-features="msDataProtection,msEndpointDlp,msIrm,msIrmv2,msMdatpWebSiteDlp,msMdatpWebSiteDlpMac,msMdatpWebSiteDlpv2,msPerformanceModeToggle,BlockInsecurePrivateNetworkRequests,BlockInsecurePrivateNetworkRequestsForNavigations,BrowserDynamicCodeDisabled,DisableProcessReuse,ElementSuperRareData,EnableCsrssLockdown,EncryptedClientHello,ForceIsolationInfoFrameOriginToTopLevelFrame,GpuAppContainer,ImprovedCookieControls,IntensiveWakeUpThrottling:grace_period_seconds/10,IsolateOrigins,IsolatePrerenders,IsolateSandboxedIframes,MinimizeAudioProcessingForUnusedOutput,NetworkServiceSandbox,NetworkServiceCodeIntegrity,OpaqueResponseBlockingV01,OriginIsolationHeader,PartitionConnectionsByNetworkIsolationKey,PartitionDomainReliabilityByNetworkIsolationKey,PartitionExpectCTStateByNetworkIsolationKey,PartitionHttpServerPropertiesByNetworkIsolationKey,PartitionNelAndReportingByNetworkIsolationKey,PartitionSSLSessionsByNetworkIsolationKey,PartitionedCookies,PostQuantumCECPQ2,PrefetchPrivacyChanges,ReduceUserAgent,ReducedReferrerGranularity,RendererAppContainer,RestrictGamepadAccess,SandboxExternalProtocolBlocked,SandboxHttpCache,ScopeMemoryCachePerContext,SplitAuthCacheByNetworkIsolationKey,SplitCacheByIncludeCredentials,SplitCacheByNetworkIsolationKey,SplitHostCacheByNetworkIsolationKey,StrictOriginIsolation,SuppressDifferentOriginSubframeJSDialogs,ThirdPartyStoragePartitioning,ThrottleForegroundTimers,UseRegistrableDomainInNetworkIsolationKey,WinSboxDisableExtensionPoint,WinSboxDisableKtmComponent" --disable-features="AcceptCHFrame,AdInterestGroupAPI,AllowClientHintsToThirdParty,AllowURNsInIframes,AutoupgradeMixedContent,BrowsingTopics,ClearCrossSiteCrossBrowsingContextGroupWindowName,ClientHintThirdPartyDelegation,ClientHintsDPR,ClientHintsDPR_DEPRECATED,ClientHintsDeviceMemory,ClientHintsDeviceMemory_DEPRECATED,ClientHintsMetaHTTPEquivAcceptCH,ClientHintsMetaNameAcceptCH,ClientHintsResourceWidth,ClientHintsResourceWidth_DEPRECATED,ClientHintsViewportWidth,ClientHintsViewportWidth_DEPRECATED,ContextMenuPerformanceInfoAndRemoteHintFetching,CopyLinkToText,CriticalClientHint,CssSelectorFragmentAnchor,DirectSockets,EnableSignedExchangePrefetchCacheForNavigations,EnableSignedExchangeSubresourcePrefetch,EnableSubresourceWebBundles,ExperimentalJSProfiler,EnableTLS13EarlyData,FedCm,Fledge,FontAccess,FontAccessPersistent,GreaseUACH,IdleDetection,InterestGroupStorage,Journeys,MediaEngagementBypassAutoplayPolicies,NTPArticleSuggestions,NotificationTriggers,OmniboxTriggerForNoStatePrefetch,Parakeet,Prerender2,PrefersColorSchemeClientHintHeader,PreloadMediaEngagementData,RetailCoupons,SegmentationPlatform,SignedExchangeReportingForDistributors,SpeculationRulesPrefetchProxy,SubresourceWebBundles,TFLiteLanguageDetectionEnabled,TextFragmentAnchor,UACHPlatformEnabledByDefault,UserAgentClientHint,UserAgentClientHintFullVersionList,UsernameFirstFlow,UsernameFirstFlowFilling,UsernameFirstFlowFallbackCrowdsourcing,ViewportHeightClientHintHeader,WebNFC,WebOTP,WebSQLInThirdPartyContextEnabled,WebXR"
```

This batch file provides hardened switches for Edge while maintaining your workflow.

## Registry value

Here is the registry value that you should copy in the (Default) string for each of the mentioned keys.

Please choose the appropriate value for your edition of Edge.

**Edge Stable:**
```
"C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" --disable-breakpad --disable-domain-reliability --disable-external-intent-requests --disable-file-system --extension-content-verification=enforce_strict --extensions-install-verification=enforce  --no-pings --process-per-site --site-per-process --enable-features="msDataProtection,msEndpointDlp,msIrm,msIrmv2,msMdatpWebSiteDlp,msMdatpWebSiteDlpMac,msMdatpWebSiteDlpv2,msPerformanceModeToggle,BlockInsecurePrivateNetworkRequests,BlockInsecurePrivateNetworkRequestsForNavigations,BrowserDynamicCodeDisabled,DisableProcessReuse,ElementSuperRareData,EnableCsrssLockdown,EncryptedClientHello,ForceIsolationInfoFrameOriginToTopLevelFrame,GpuAppContainer,ImprovedCookieControls,IntensiveWakeUpThrottling:grace_period_seconds/10,IsolateOrigins,IsolatePrerenders,IsolateSandboxedIframes,MinimizeAudioProcessingForUnusedOutput,NetworkServiceSandbox,NetworkServiceCodeIntegrity,OpaqueResponseBlockingV01,OriginIsolationHeader,PartitionConnectionsByNetworkIsolationKey,PartitionDomainReliabilityByNetworkIsolationKey,PartitionExpectCTStateByNetworkIsolationKey,PartitionHttpServerPropertiesByNetworkIsolationKey,PartitionNelAndReportingByNetworkIsolationKey,PartitionSSLSessionsByNetworkIsolationKey,PartitionedCookies,PostQuantumCECPQ2,PrefetchPrivacyChanges,ReduceUserAgent,ReducedReferrerGranularity,RendererAppContainer,RestrictGamepadAccess,SandboxExternalProtocolBlocked,SandboxHttpCache,ScopeMemoryCachePerContext,SplitAuthCacheByNetworkIsolationKey,SplitCacheByIncludeCredentials,SplitCacheByNetworkIsolationKey,SplitHostCacheByNetworkIsolationKey,StrictOriginIsolation,SuppressDifferentOriginSubframeJSDialogs,ThirdPartyStoragePartitioning,ThrottleForegroundTimers,UseRegistrableDomainInNetworkIsolationKey,WinSboxDisableExtensionPoint,WinSboxDisableKtmComponent" --disable-features="AcceptCHFrame,AdInterestGroupAPI,AllowClientHintsToThirdParty,AllowURNsInIframes,AutoupgradeMixedContent,BrowsingTopics,ClearCrossSiteCrossBrowsingContextGroupWindowName,ClientHintThirdPartyDelegation,ClientHintsDPR,ClientHintsDPR_DEPRECATED,ClientHintsDeviceMemory,ClientHintsDeviceMemory_DEPRECATED,ClientHintsMetaHTTPEquivAcceptCH,ClientHintsMetaNameAcceptCH,ClientHintsResourceWidth,ClientHintsResourceWidth_DEPRECATED,ClientHintsViewportWidth,ClientHintsViewportWidth_DEPRECATED,ContextMenuPerformanceInfoAndRemoteHintFetching,CopyLinkToText,CriticalClientHint,CssSelectorFragmentAnchor,DirectSockets,EnableSignedExchangePrefetchCacheForNavigations,EnableSignedExchangeSubresourcePrefetch,EnableSubresourceWebBundles,ExperimentalJSProfiler,EnableTLS13EarlyData,FedCm,Fledge,FontAccess,FontAccessPersistent,GreaseUACH,IdleDetection,InterestGroupStorage,Journeys,MediaEngagementBypassAutoplayPolicies,NTPArticleSuggestions,NotificationTriggers,OmniboxTriggerForNoStatePrefetch,Parakeet,Prerender2,PrefersColorSchemeClientHintHeader,PreloadMediaEngagementData,RetailCoupons,SegmentationPlatform,SignedExchangeReportingForDistributors,SpeculationRulesPrefetchProxy,SubresourceWebBundles,TFLiteLanguageDetectionEnabled,TextFragmentAnchor,UACHPlatformEnabledByDefault,UserAgentClientHint,UserAgentClientHintFullVersionList,UsernameFirstFlow,UsernameFirstFlowFilling,UsernameFirstFlowFallbackCrowdsourcing,ViewportHeightClientHintHeader,WebNFC,WebOTP,WebSQLInThirdPartyContextEnabled,WebXR" --single-attribute %1
```

**Edge Beta:**
```
"C:\Program Files (x86)\Microsoft\Edge Beta\Application\msedge.exe" --disable-breakpad --disable-domain-reliability --disable-external-intent-requests --disable-file-system --extension-content-verification=enforce_strict --extensions-install-verification=enforce  --no-pings --process-per-site --site-per-process --enable-features="msDataProtection,msEndpointDlp,msIrm,msIrmv2,msMdatpWebSiteDlp,msMdatpWebSiteDlpMac,msMdatpWebSiteDlpv2,msPerformanceModeToggle,BlockInsecurePrivateNetworkRequests,BlockInsecurePrivateNetworkRequestsForNavigations,BrowserDynamicCodeDisabled,DisableProcessReuse,ElementSuperRareData,EnableCsrssLockdown,EncryptedClientHello,ForceIsolationInfoFrameOriginToTopLevelFrame,GpuAppContainer,ImprovedCookieControls,IntensiveWakeUpThrottling:grace_period_seconds/10,IsolateOrigins,IsolatePrerenders,IsolateSandboxedIframes,MinimizeAudioProcessingForUnusedOutput,NetworkServiceSandbox,NetworkServiceCodeIntegrity,OpaqueResponseBlockingV01,OriginIsolationHeader,PartitionConnectionsByNetworkIsolationKey,PartitionDomainReliabilityByNetworkIsolationKey,PartitionExpectCTStateByNetworkIsolationKey,PartitionHttpServerPropertiesByNetworkIsolationKey,PartitionNelAndReportingByNetworkIsolationKey,PartitionSSLSessionsByNetworkIsolationKey,PartitionedCookies,PostQuantumCECPQ2,PrefetchPrivacyChanges,ReduceUserAgent,ReducedReferrerGranularity,RendererAppContainer,RestrictGamepadAccess,SandboxExternalProtocolBlocked,SandboxHttpCache,ScopeMemoryCachePerContext,SplitAuthCacheByNetworkIsolationKey,SplitCacheByIncludeCredentials,SplitCacheByNetworkIsolationKey,SplitHostCacheByNetworkIsolationKey,StrictOriginIsolation,SuppressDifferentOriginSubframeJSDialogs,ThirdPartyStoragePartitioning,ThrottleForegroundTimers,UseRegistrableDomainInNetworkIsolationKey,WinSboxDisableExtensionPoint,WinSboxDisableKtmComponent" --disable-features="AcceptCHFrame,AdInterestGroupAPI,AllowClientHintsToThirdParty,AllowURNsInIframes,AutoupgradeMixedContent,BrowsingTopics,ClearCrossSiteCrossBrowsingContextGroupWindowName,ClientHintThirdPartyDelegation,ClientHintsDPR,ClientHintsDPR_DEPRECATED,ClientHintsDeviceMemory,ClientHintsDeviceMemory_DEPRECATED,ClientHintsMetaHTTPEquivAcceptCH,ClientHintsMetaNameAcceptCH,ClientHintsResourceWidth,ClientHintsResourceWidth_DEPRECATED,ClientHintsViewportWidth,ClientHintsViewportWidth_DEPRECATED,ContextMenuPerformanceInfoAndRemoteHintFetching,CopyLinkToText,CriticalClientHint,CssSelectorFragmentAnchor,DirectSockets,EnableSignedExchangePrefetchCacheForNavigations,EnableSignedExchangeSubresourcePrefetch,EnableSubresourceWebBundles,ExperimentalJSProfiler,EnableTLS13EarlyData,FedCm,Fledge,FontAccess,FontAccessPersistent,GreaseUACH,IdleDetection,InterestGroupStorage,Journeys,MediaEngagementBypassAutoplayPolicies,NTPArticleSuggestions,NotificationTriggers,OmniboxTriggerForNoStatePrefetch,Parakeet,Prerender2,PrefersColorSchemeClientHintHeader,PreloadMediaEngagementData,RetailCoupons,SegmentationPlatform,SignedExchangeReportingForDistributors,SpeculationRulesPrefetchProxy,SubresourceWebBundles,TFLiteLanguageDetectionEnabled,TextFragmentAnchor,UACHPlatformEnabledByDefault,UserAgentClientHint,UserAgentClientHintFullVersionList,UsernameFirstFlow,UsernameFirstFlowFilling,UsernameFirstFlowFallbackCrowdsourcing,ViewportHeightClientHintHeader,WebNFC,WebOTP,WebSQLInThirdPartyContextEnabled,WebXR" --single-attribute %1
```

**Edge Dev:**
```
"C:\Program Files (x86)\Microsoft\Edge Dev\Application\msedge.exe" --disable-breakpad --disable-domain-reliability --disable-external-intent-requests --disable-file-system --extension-content-verification=enforce_strict --extensions-install-verification=enforce  --no-pings --process-per-site --site-per-process --enable-features="msDataProtection,msEndpointDlp,msIrm,msIrmv2,msMdatpWebSiteDlp,msMdatpWebSiteDlpMac,msMdatpWebSiteDlpv2,msPerformanceModeToggle,BlockInsecurePrivateNetworkRequests,BlockInsecurePrivateNetworkRequestsForNavigations,BrowserDynamicCodeDisabled,DisableProcessReuse,ElementSuperRareData,EnableCsrssLockdown,EncryptedClientHello,ForceIsolationInfoFrameOriginToTopLevelFrame,GpuAppContainer,ImprovedCookieControls,IntensiveWakeUpThrottling:grace_period_seconds/10,IsolateOrigins,IsolatePrerenders,IsolateSandboxedIframes,MinimizeAudioProcessingForUnusedOutput,NetworkServiceSandbox,NetworkServiceCodeIntegrity,OpaqueResponseBlockingV01,OriginIsolationHeader,PartitionConnectionsByNetworkIsolationKey,PartitionDomainReliabilityByNetworkIsolationKey,PartitionExpectCTStateByNetworkIsolationKey,PartitionHttpServerPropertiesByNetworkIsolationKey,PartitionNelAndReportingByNetworkIsolationKey,PartitionSSLSessionsByNetworkIsolationKey,PartitionedCookies,PostQuantumCECPQ2,PrefetchPrivacyChanges,ReduceUserAgent,ReducedReferrerGranularity,RendererAppContainer,RestrictGamepadAccess,SandboxExternalProtocolBlocked,SandboxHttpCache,ScopeMemoryCachePerContext,SplitAuthCacheByNetworkIsolationKey,SplitCacheByIncludeCredentials,SplitCacheByNetworkIsolationKey,SplitHostCacheByNetworkIsolationKey,StrictOriginIsolation,SuppressDifferentOriginSubframeJSDialogs,ThirdPartyStoragePartitioning,ThrottleForegroundTimers,UseRegistrableDomainInNetworkIsolationKey,WinSboxDisableExtensionPoint,WinSboxDisableKtmComponent" --disable-features="AcceptCHFrame,AdInterestGroupAPI,AllowClientHintsToThirdParty,AllowURNsInIframes,AutoupgradeMixedContent,BrowsingTopics,ClearCrossSiteCrossBrowsingContextGroupWindowName,ClientHintThirdPartyDelegation,ClientHintsDPR,ClientHintsDPR_DEPRECATED,ClientHintsDeviceMemory,ClientHintsDeviceMemory_DEPRECATED,ClientHintsMetaHTTPEquivAcceptCH,ClientHintsMetaNameAcceptCH,ClientHintsResourceWidth,ClientHintsResourceWidth_DEPRECATED,ClientHintsViewportWidth,ClientHintsViewportWidth_DEPRECATED,ContextMenuPerformanceInfoAndRemoteHintFetching,CopyLinkToText,CriticalClientHint,CssSelectorFragmentAnchor,DirectSockets,EnableSignedExchangePrefetchCacheForNavigations,EnableSignedExchangeSubresourcePrefetch,EnableSubresourceWebBundles,ExperimentalJSProfiler,EnableTLS13EarlyData,FedCm,Fledge,FontAccess,FontAccessPersistent,GreaseUACH,IdleDetection,InterestGroupStorage,Journeys,MediaEngagementBypassAutoplayPolicies,NTPArticleSuggestions,NotificationTriggers,OmniboxTriggerForNoStatePrefetch,Parakeet,Prerender2,PrefersColorSchemeClientHintHeader,PreloadMediaEngagementData,RetailCoupons,SegmentationPlatform,SignedExchangeReportingForDistributors,SpeculationRulesPrefetchProxy,SubresourceWebBundles,TFLiteLanguageDetectionEnabled,TextFragmentAnchor,UACHPlatformEnabledByDefault,UserAgentClientHint,UserAgentClientHintFullVersionList,UsernameFirstFlow,UsernameFirstFlowFilling,UsernameFirstFlowFallbackCrowdsourcing,ViewportHeightClientHintHeader,WebNFC,WebOTP,WebSQLInThirdPartyContextEnabled,WebXR" --single-attribute %1
```

## Switches

| Name | Description |
| :--- | :---------- |
| --disable-domain-reliability | Disables Domain Reliability Monitoring which is unnecessary |
| --disable-external-intent-requests | Never forward URL requests to external intents |
| --disable-file-system | Disables the bleeding edge FileSystem API |
| --extension-content-verification | Ensures extension verification |
| --extensions-install-verification | Ditto |
| --no-pings | Blocks hyperlink auditing pings |
| --process-per-site | Bundles same-site pages to share a single process |
| --site-per-process | Enforces a one-site-per-process security policy |

## Enabled Features

Partitioning:
* ForceIsolationInfoFrameOriginToTopLevelFrame
* IsolateOrigins
* IsolatePrerenders
* IsolateSandboxedIframes
* OriginIsolationHeader
* PartitionConnectionsByNetworkIsolationKey
* PartitionDomainReliabilityByNetworkIsolationKey
* PartitionExpectCTStateByNetworkIsolationKey
* PartitionHttpServerPropertiesByNetworkIsolationKey
* PartitionNelAndReportingByNetworkIsolationKey
* PartitionSSLSessionsByNetworkIsolationKey
* PartitionedCookies
* SandboxHttpCache
* SplitAuthCacheByNetworkIsolationKey
* SplitCacheByIncludeCredentials
* SplitCacheByNetworkIsolationKey
* SplitHostCacheByNetworkIsolationKey
* StrictOriginIsolation
* UseRegistrableDomainInNetworkIsolationKey
	
Sandboxing:
* BrowserDynamicCodeDisabled
	* Prevents the browser process from generating dynamic code or modifying executable code using ACG
* EnableCsrssLockdown
* GpuAppContainer
* NetworkServiceCodeIntegrity
	* Strengthens CIG (Control Integrity Guard) mitigation in the network process
* NetworkServiceSandbox
	* Strengthens ACG (Arbitrary Code Guard) mitigation in the network process
* RendererAppContainer
* SandboxExternalProtocolBlocked
* WinSboxDisableExtensionPoint
* WinSboxDisableKtmComponent

Privacy & Security:
* AutoupgradeMixedContent
* BlockInsecurePrivateNetworkRequests, BlockInsecurePrivateNetworkRequestsForNavigations
	* Blocks insecure private network requests
* ClearCrossSiteCrossBrowsingContextGroupWindowName
* DisableProcessReuse, ReduceUserAgent
* EncryptedClientHello
* ImprovedCookieControls
	* Improved third-party cookie blocking.
* OpaqueResponseBlockingV01
	* [Documentation](https://docs.google.com/document/d/1qUbE2ySi6av3arUEw5DNdFJIKKBbWGRGsXz_ew3S7HQ)
* PostQuantumCECPQ2
* PrefetchPrivacyChanges
	* Prefetch requests will not follow redirects, not send a header, not send credentials, and do not pass through service workers
* ReducedReferrerGranularity
	* Enables strict-origin-when-cross-origin

## Disabled Features

PrivacySandbox/FloC Related:
* AdInterestGroupAPI
* AllowURNsInIframes
* BrowsingTopics
* FedCm
* Fledge
* InterestGroupStorage
* Parakeet

SXG:
* EnableSignedExchangePrefetchCacheForNavigations
* EnableSignedExchangeSubresourcePrefetch
* SignedExchangeReportingForDistributors

WebBundles:
* EnableSubresourceWebBundles
* SubresourceWebBundles

ClientHints:
* AcceptCHFrame
* AllowClientHintsToThirdParty
* ClientHintThirdPartyDelegation
* ClientHintsDPR
* ClientHintsDPR_DEPRECATED
* ClientHintsDeviceMemory
* ClientHintsDeviceMemory_DEPRECATED
* ClientHintsMetaHTTPEquivAcceptCH
* ClientHintsMetaNameAcceptCH
* ClientHintsResourceWidth
* ClientHintsResourceWidth_DEPRECATED
* ClientHintsViewportWidth
* ClientHintsViewportWidth_DEPRECATED
* CriticalClientHint
* GreaseUACH
* PrefersColorSchemeClientHintHeader
* UACHPlatformEnabledByDefault
* UserAgentClientHint
* UserAgentClientHintFullVersionList
* ViewportHeightClientHintHeader

Others:
* CssSelectorFragmentAnchor
* DirectSockets
* EnableTLS13EarlyData
* ExperimentalJSProfiler
* FontAccess, FontAccessPersistent
* IdleDetection
* Journeys
* NTPArticleSuggestions
* NotificationTriggers
* OmniboxTriggerForNoStatePrefetch
* PreloadMediaEngagementData, MediaEngagementBypassAutoplayPolicies
* Prerender2
* RetailCoupons
* SegmentationPlatform
* SpeculationRulesPrefetchProxy
* TFLiteLanguageDetectionEnabled
* TextFragmentAnchor, CopyLinkToText
	* Disables text snippets in URL fragments
* UsernameFirstFlow, UsernameFirstFlowFilling, UsernameFirstFlowFallbackCrowdsourcing
* WebNFC, WebOTP, WebXR
	* Blocks NFC, OTP and XR APIs
* WebSQLInThirdPartyContextEnabled

## MS Edge specific feature flags

Enabled:
* msDataProtection, msEndpointDlp, msMdatpWebSiteDlp, msMdatpWebSiteDlpv2, msMdatpWebSiteDlpMac, msIrm, msIrmv2
	* Feature Flags for Data Loss Prevention `edge://edge-dlp-internals/`
