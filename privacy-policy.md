# Gophr Privacy Policy

Last updated: October 13, 2026

This policy explains how Gophr for iPhone and Apple Watch handles your information and describes its companion website. “We” and “us” mean the developer of Gophr.

Gophr records walks, runs, cycles, and drives and creates a personal activity history and heatmap. Your activity history is stored on your devices. You do not need a Gophr account, and we do not operate a server that receives your activity history. Optional Apple services, backups, exports, and support communications are described below.

## Information Gophr accesses and how it is used

### Location and activity information

With your permission, Gophr accesses location through your iPhone or Apple Watch to show your position and record activities. Recorded information includes precise coordinates, timestamps, elevation, location accuracy, speed, and direction when available. During an active recording, location access can continue in the background or while the screen is locked.

Gophr stores activity type, start and end times, recording events such as pauses, route points, and calculated information such as duration, distance, pace, and elevation gain. It uses this information to record and recover interrupted activities, display and edit activity history, smooth routes, generate route thumbnails and elevation views, and build your personal heatmap. These activity calculations and history processing take place on your devices.

You can also enter activity names, notes, dates, and manually drawn or edited routes. If you import a backup, Gophr reads the activity information in the file you select and stores it locally for these same purposes.

### Location permission choices

Onboarding and browsing do not require location permission. Gophr explains and requests location access when you choose GPS recording or current location. Recording may request precise and background access to preserve your route while the screen is locked. Denying location leaves manual entries, history, backups, and exports available. Gophr does not request Motion & Fitness permission or collect Core Motion activity readings.

### Apple Health

If you enable **Export workouts to Apple Health** and grant the relevant permissions, Gophr uses HealthKit on your paired Apple Watch for eligible walks, runs, and cycles. This includes Watch-started workouts and iPhone-started workouts mirrored to the Watch. Drive activities are not exported as fitness workouts. It requests access to read heart rate, active energy burned, walking/running distance, and cycling distance, and permission to save workouts, workout routes, active energy, and distance. Available measurements are used to support the active workout and its record in Apple Health and Fitness.

Health access is optional. Gophr does not use HealthKit information for advertising, marketing, data brokerage, or unrelated profiling, and does not send it to a Gophr server. Apple controls storage and any synchronization of your Health records under your Apple settings.

### Settings and operational information

Gophr stores preferences such as units, map options, and Health export settings, along with recording recovery state, activity identifiers, synchronization status, and backup status. If you select a backup folder, it stores a system-provided reference that allows access to that folder. This information supports your preferences, reliable recording, device synchronization, and the backup features you choose.

Gophr can generate local diagnostic logs containing technical events, activity identifiers, timestamps, and error details to help troubleshoot recording, synchronization, and Health export. Gophr has no third-party advertising, tracking, or analytics service. Apple may provide crash reports, diagnostics, or TestFlight feedback according to your Apple settings and Apple's policies. We use reports we receive to diagnose problems and improve reliability.

### Purchases and free activity allowance

Gophr uses Apple's StoreKit to offer the one-time **Gophr_full** purchase. Apple processes payment and provides signed purchase and entitlement information, including the product identifier, transaction status, and revocation status. Gophr verifies this information on your device to unlock activity recording, manual entry creation and editing, and backup imports after the free 20 km allowance. We do not receive your payment card details or send your activity history to Apple for purchase verification. Apple retains purchase records under its own policies; deleting Gophr does not delete your App Store purchase history.

Gophr stores activity identifiers and the highest distance counted for each activity locally to measure cumulative use of the free allowance. Shortening or deleting activities, clearing local activity data, or importing an older backup does not reset that allowance. The paired iPhone and Apple Watch exchange these usage records and purchase access status to apply the limit on both devices. These records are not sent to a developer-operated server. Usage records remain until the app is deleted from the relevant device; device backups and paired-device synchronization may restore them. History viewing and data exports remain available without purchasing. Gophr does not offer ad-supported access or include an advertising SDK.

### Information you send to support

If you contact us, we receive the contact details, message, and any files or diagnostics you choose to provide. We use them to respond, troubleshoot, and handle privacy requests. You do not need to send your activity history or Health information to ask a privacy question.

## Coverage goals and network downloads

Goals is available in development and internal TestFlight branch builds. It is hidden in external TestFlight and production branch builds. In Goals, you can draw polygons or circles, give them names, choose eligible activity types, and configure a network dataset URL. Gophr stores these goal definitions and their dataset version locally. It reads saved activity coordinates, timestamps, accuracy and pause/filter flags from local history to estimate the unique walking-network distance covered inside each area. Repeated travel does not earn duplicate coverage. Route matching and coverage calculations take place on the iPhone; goal polygons and activity history are not uploaded to the tile host.

Opening or calculating a configured goal downloads a static manifest and the road/path tiles needed for that area over HTTPS. The bucket/CDN operator receives the device's IP address, request time and requested file paths; tile paths reveal the approximate geographic area requested. These requests deliver network data and may be logged by the host for service operation and security. Gophr sends no account identifier, activity identifier, route trace, goal name or exact polygon with those requests and uses no advertising or analytics SDK for Goals. Apple MapKit also provides the basemap under the map practices described below.

Goal definitions remain locally until you delete them in Goals or use Settings → Clear local data. Clearing local data removes the saved goals and dataset URLs together with other settings. The current activity backup and export formats do not include goal definitions or dataset settings. Coverage results are temporary and are recalculated from saved activities, excluding deleted and discarded activities. Downloaded public network files are kept in a size-limited device cache and may be evicted by Gophr or iOS; deleting the app removes this cache. Cached network files contain no activity history or polygon definitions.

To stop future tile requests, leave Goals or remove its dataset URL. Leaving Goals cancels its calculation after any in-flight download or computation finishes. Deleting a goal does not delete your activities. For a host you configure independently, consult that provider's retention policy and request deletion of request logs from that provider. Any host we select to deliver Gophr data must provide the same or equal protection described in this policy and required by Apple's guidelines, including limits on use, retention and deletion. We use any request logs we receive only as long as necessary for delivery, troubleshooting and security, and you may request deletion through the contact method below.

## Companion website and policy links

The companion Gophr website loads fonts from Google Fonts. Visiting it can send Google your IP address and browser/request information needed to retrieve those fonts. This website font loading is separate from the native app, which does not load Google Fonts. The checked website contains no advertising or analytics integration. The website host may receive ordinary page-request information; its handling depends on the host's own practices.

Opening a policy, attribution, or support link launches the relevant website, such as GitHub, Apple, or OpenStreetMap. That website receives normal web-request information and handles it under its own privacy terms. Opening these links does not attach your Gophr activity database, route history, or Health records.

## When information leaves your device

- **Your paired devices:** Gophr uses Apple's device connectivity services to exchange recording controls, settings, activity status, and recorded routes between your iPhone and Apple Watch. Watch recordings are retained locally while awaiting transfer to your iPhone.
- **Apple Maps:** Gophr uses Apple's MapKit to display maps. Loading maps can send requests to Apple, including the map area requested and network information such as your IP address. Apple's handling of map-service information is explained in [Apple Maps & Privacy](https://www.apple.com/legal/privacy/data/en/apple-maps/).
- **Apple Health:** When you enable Health export and authorize access, workout information and routes are saved to Apple Health. Other apps can access those records only as permitted by your Health sharing settings.
- **Backups and exports you choose:** Gophr writes activity data to the folder or export destination you select. If that destination uses iCloud Drive or another storage provider, that provider may upload and store the files. Automatic backups write to your chosen folder when enabled. Backup and export files can contain precise routes, activity details, notes, and retained records of deleted activities. Importing a backup reads from the location you select.
- **Device backups:** Depending on your device settings, Apple's device backup or transfer features may copy app data independently of Gophr's optional backup feature.
- **Support and diagnostics:** Information you submit to support, and diagnostics made available through Apple, may be received by us as described above.

We do not sell or rent your personal information, share it for targeted advertising, or track you across other companies' apps and websites. We do not give advertisers, data brokers, or affiliated companies access to your activity history.

Any third party with whom we share user data to provide Gophr, including service providers, third-party SDK providers, and any parent, subsidiary, or related entity given access, must provide the same or equal protection of that data as described in this policy and required by Apple's App Review Guidelines. This requirement applies to their use, security, retention, and deletion of the data. Gophr does not authorize those recipients to use your data for their own advertising or unrelated purposes.

When you independently choose a storage provider or share an exported file with someone else, that recipient's privacy terms and your sharing settings also apply. [Apple's Privacy Policy](https://www.apple.com/legal/privacy/) describes Apple's services.

## Retention and deletion

**On-device history:** Gophr retains activity history on your device until you remove it. There is no automatic expiration period. Deleting an individual activity hides it from normal history and map views, but is a **soft delete**: the underlying activity and route records can remain in local storage and can be included in backups and exports. Discarded recordings can also leave local records.

**Clear local data:** To remove the activity records, route points, recording events, summaries, and derived map data from Gophr's iPhone data store, open **Settings → Clear local data → Delete local data**. This also clears settings stored in that data store. It does not clear the separately stored free-allowance usage records or revoke an App Store purchase. It does not delete copies in Apple Health, backup folders, exported files, device backups, or on your Apple Watch. It is not a secure-erasure guarantee for underlying device storage.

**Apple Watch:** After the iPhone acknowledges an imported Watch recording, Gophr removes the corresponding Watch route points and recording events; some activity metadata and preferences can remain. An iPhone data reset does not reset the Watch app. To remove remaining Watch app data, delete Gophr from the Watch as well. Pending Watch transfers or later backup imports can bring activity data back to the iPhone.

**Backups and exports:** These remain in the locations you chose until you delete them. Turning off automatic backups or clearing local data does not remove existing files. Delete those files through Files or your storage provider, including any recently deleted items or retained versions. Manage device backups separately in Apple's backup settings. Temporary files used to prepare imports or exports can remain in the app's temporary storage until cleaned up by the app or operating system, or until the app is deleted.

**Apple Health:** Deleting an activity in Gophr, clearing Gophr's local data, disabling export, or uninstalling Gophr does not delete previously saved Health records. Use the Health app's data management controls to delete Gophr's workouts, routes, and associated measurements.

**App removal:** Deleting the app removes its local app data on that device; offloading an app can retain its data. Copies on other devices or in Health, exports, or backups must be removed separately.

**Support and diagnostics:** We retain information we receive only as long as needed to resolve your request, investigate the reported issue, or meet a legal obligation. You can request deletion through the contact method below. If a legal obligation requires retention, we will explain the applicable limitation. We cannot remotely access or erase activity history stored only on your devices or in storage accounts you control.

## Your choices and withdrawing permission

- Change or revoke Gophr's location permission, including precise location and background access, in your device's **Settings → Privacy & Security → Location Services**. This may limit location display and route recording.
- Turn off **Export workouts to Apple Health** in Gophr's Settings and manage Gophr's read and write permissions in Apple Health. Stop an active workout before changing export settings if you want it to stop using Health.
- Turn off **Automatic** in Gophr's **Settings → Backup** to stop future automatic backups.
- Use **Settings → Backup → Export data** to obtain a copy of your activity data, and the deletion controls described above to remove it.
- Manage whether activity information appears on your Lock Screen, Dynamic Island, or Watch widgets using Apple's Live Activity, notification, and widget settings. These surfaces can show activity details to someone who can see your device. The CarPlay preview available in development and internal TestFlight builds displays existing recording and map information on the iPhone; it does not introduce a separate account or developer-operated upload service.

Device menu names may vary by operating system version. Withdrawing permission stops future access governed by that permission; it does not automatically erase information already recorded or shared.

## Security

Gophr uses Apple's app sandbox and system permission controls to restrict access to app data and device features. Backup and export archives are not password-protected by Gophr. Protect your devices and chosen storage accounts, and share exported routes carefully because they can reveal sensitive places and routines. No storage or transfer method can guarantee absolute security.

## Policy changes

We will update this policy when Gophr's data practices change and revise the date above. If a change requires additional permission, we will request it before accessing or using your information in that way.

## Contact and privacy requests

To ask a privacy question or request deletion of information you have sent us, contact the developer through the **App Support** link on Gophr's App Store product page. For TestFlight builds, you can also use **Send Beta Feedback** in TestFlight. Identify your request as a Gophr privacy request and describe the information involved without including unnecessary location or Health data.

