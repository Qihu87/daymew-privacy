# DayMew Privacy Policy

Last updated: October 29, 2026

DayMew (“the app,” “we,” or “us”) is a habit tracking and check-in app. This policy explains how data is stored, used, synchronized, and otherwise processed when you use the app, and the choices available to you.

The app does not have an independent account registration or sign-in system, and we do not operate our own business servers to centrally store your habits, journals, or photos. Core habit data is stored on your device. If you enable iCloud Sync, relevant data is also synchronized to your personal iCloud private database.

We use Mixpanel for product usage analytics and RevenueCat for purchase status synchronization and purchase analytics. Keeping core habit content off developer-operated servers does not mean that no information leaves your device. These activities are explained separately below.

## 1. Data you create in the app

Depending on the features you use, the app stores the following information on your device to provide habit management, check-ins, reminders, and statistics:

- Habit information: a selected preset or custom name, habit type, icon, color, notes, tags, start and end dates, repeat rules, reminder times, goals, photo requirements, archive status, and related settings.
- Check-in information: dates, completed or skipped status, quantities, durations, completion times, journal text, photos, and related progress.
- Bad-habit records: events you choose to record, their times, counts, quantities, units, or durations.
- Derived feature data: coin rewards, statistics, and display states associated with these records.

Habit names, journals, and photos may contain personal information you choose to enter or capture, including faces, text, and information about health, religion, or other private aspects of your life. Whether information is sensitive personal data depends on its content and applicable law. This content is used only for the habit recording, check-in, display, statistics, and optional synchronization features you choose to use. It is not used for advertising, sent to Mixpanel or RevenueCat as analytics events or user attributes, or uploaded to our own business servers.

## 2. Local profile and preferences

The app stores your nickname, avatar choice, custom avatar image, appearance preferences, notification master setting, first day of the week, check-in sound, and local states needed for membership features and offer presentation on your device.

It also stores the date you first created a habit to display how long you have been using the app. Deleting an individual habit does not reset that date.

Your nickname, custom avatar, appearance, and notification master setting are not included in the current CloudKit habit-data synchronization. The first-day-of-week setting can synchronize when iCloud Sync is enabled.

## 3. iCloud Sync

iCloud Sync is a Pro feature. You need an active Pro membership to enable it.

If you enable iCloud Sync and your device is signed in to an available Apple Account, the app uses Apple's iCloud / CloudKit services to synchronize relevant data, including:

- Habits and their settings;
- Check-in progress, journals, and bad-habit events;
- Tags;
- Check-in photos;
- Your first-day-of-week setting.

This data is synchronized to your personal CloudKit private database to keep devices signed in to the same Apple Account consistent. The developer cannot view the contents of other users' private databases through the CloudKit developer dashboard.

Synchronizing check-in photos requires uploading them to Apple's services. Once synchronization is enabled, those photos are no longer stored only on a single device.

You can turn off iCloud Sync in the app's settings. Turning it off does not actively delete data already stored in iCloud. Availability and completion of synchronization depend on factors such as your network, device state, iCloud storage space, and Apple's services.

Apple's handling of iCloud services is also subject to its applicable terms and privacy policy:

[Apple Privacy Policy](https://www.apple.com/legal/privacy/)

## 4. Camera, photos, notifications, and alarm permissions

### Camera

When you open the check-in camera screen, the app requests camera permission if needed to take check-in photos. Turning on a habit's photo check-in requirement alone does not request camera permission in advance. If you decline permission, you cannot take photos in the app, but other features that do not require the camera remain available.

### Photos

When you select photos from the photo library within the check-in camera screen, the app requests photo-library read access and uses the system photo picker. You choose the access scope through the options provided by iOS and can change it in system settings.

When setting a custom avatar, the app uses the system photo picker to obtain the image you choose.

Photos taken or selected for check-ins are re-encoded as JPEG and saved in the app's own storage, along with processed custom avatar images. The app does not request permission to write to the system photo library and does not save an additional copy of check-in photos there. When you enable iCloud Sync, check-in photos synchronize to your personal iCloud private database as described in Section 3; custom avatars do not synchronize with habit data. System backups are a separate system mechanism described in Section 9.

Re-encoding does not guarantee removal of all metadata. We do not promise that all GPS, EXIF, or other metadata has been removed.

### Notifications

The app may request notification permission when it needs to schedule local notifications. This includes enabling daily reminders, saving a habit with reminders, or saving an unfinished good habit that triggers scheduling of a daily results summary. Scheduling the daily results summary may request permission even if that habit's own reminder is turned off. When permission has already been granted, the app can also schedule timer-completion reminders. Notification content may include habit names; manage lock-screen notification previews according to your preferences.

These everyday reminders are scheduled on your device. We do not operate our own remote push server to send reminders containing your habit content. iCloud synchronization may use Apple's background notification mechanisms for a different purpose.

### Alarms

Only on iOS 26 or later, when you enable and use alarm reminders, the app requests system alarm authorization as needed. Without authorization, the relevant alarm feature is unavailable. Earlier system versions do not request this authorization and use ordinary notification reminders where supported by the app.

You can manage these permissions in iOS system settings at any time. Declining or withdrawing permission affects the relevant feature and does not authorize us to collect unrelated data.

## 5. In-app purchases and RevenueCat

The app offers monthly and annual auto-renewing memberships and one-time lifetime membership options through Apple's App Store. Transactions, payments, and purchase restoration use Apple's StoreKit / App Store systems.

The app obtains purchase and entitlement states through StoreKit to determine access to membership features. We do not directly obtain or store your debit or credit card numbers, Apple Account password, or complete payment credentials.

We also use RevenueCat to record, synchronize, and analyze purchase status, helping us understand membership purchases, renewals, cancellations, expirations, and refunds. In-app membership access is determined solely by App Store transaction states verified through StoreKit. RevenueCat does not participate in Pro entitlement decisions or control whether membership features are enabled or disabled.

For these purposes, RevenueCat receives purchase-related information, which may include an app user identifier, product identifiers, transaction or receipt information, purchase and expiration times, subscription status, restoration and refund information, and necessary app and device technical information. An app user identifier used by the SDK is not the nickname you enter in the app or your Apple Account password.

We have configured App Store Server Notifications in App Store Connect. Apple can send transaction status updates, such as renewals, cancellation of auto-renewal, expirations, and refunds, to RevenueCat even when the app is not open, so that related purchase records can be updated.

We do not intentionally send RevenueCat your habit names, notes, journals, check-in photos, custom avatar, or nickname.

[RevenueCat Privacy and Data Processing Information](https://www.revenuecat.com/privacy)

## 6. Product usage analytics and Mixpanel

We use Mixpanel to understand feature usage and purchase flows and improve the app. For example, we analyze whether users open the app, see a paywall, encounter a membership restriction, or complete or cancel a purchase.

The events currently sent cover:

- App opens;
- Paywall views, their source, membership tier, and related attributes;
- The type of feature blocked by a free-version limit;
- Purchase started, succeeded, and cancelled by the user, along with the product type, including discounted lifetime options;
- Taps on restore purchases.

The app does not currently send separate analytics events for failed or pending purchases.

Events may include SDK identifiers used to distinguish activity, event times, app version, operating system, device model, and attributes we configure, such as source or product type. Even without a name or email address, these identifiers may link activity from the same device or installation. We therefore do not describe this information as completely anonymous.

The current configuration disables Mixpanel's automatic event collection and IP-based geolocation. Analytics requests are sent to Mixpanel's EU regional endpoint. Disabling IP-based geolocation does not mean a service cannot receive an IP address as part of a network connection.

We do not send habit names, notes, journals, photos, custom avatars, or nickname text to Mixpanel for product analytics, and we do not use your habit content to create advertising profiles.

The app currently contains no third-party advertising SDK and does not request cross-app advertising tracking authorization.

The current version has no in-app switch to turn off Mixpanel analytics. To object to analytics or request restriction or deletion of related data, contact the email address below. Sending an email does not immediately disable the SDK in your current installation; the events described above may still be sent while the app continues to run. Stopping use of and deleting the app stops future app event reporting from that installation, but does not automatically delete information already sent.

[Mixpanel Privacy Statement](https://mixpanel.com/legal/privacy-policy/)

## 7. Feedback, websites, and external services

When you use the app's email feedback link, the system opens your mail app. You decide whether to send a message and what text, images, or other attachments to include. We receive the email address and content you send to reply, investigate issues, or handle privacy requests.

Please send only what is necessary to address your request. Opening the feedback link does not automatically attach your habits or photos to an email.

The app may include links to Apple's standard terms and social platforms such as WeChat, Xiaohongshu, X, and Threads. If you choose to open them, those websites or services may receive information necessary for network communication and process it under their own rules.

The app's Terms of Use are Apple's Standard End User License Agreement (EULA). That agreement and this privacy policy are separate documents, presented through separate links.

The privacy policy website is hosted on GitHub Pages. When you visit it, GitHub logs visitors' IP addresses for security purposes. Website visits and the storage of habit data in the app are separate processing contexts.

[GitHub Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement)

## 8. Data sharing and processing locations

We do not sell your habits, journals, or photos. We use the following services to provide the functions described in this policy:

| Service | Purpose | Main data involved |
| --- | --- | --- |
| Apple iCloud / CloudKit | Cross-device synchronization you enable | Habits, progress, journals, events, tags, check-in photos, first day of the week |
| Apple App Store / StoreKit | Payments, purchase restoration, and membership verification | Products, transactions, and membership states |
| RevenueCat | Purchase status synchronization and purchase analytics | Purchase records, app user identifiers, and necessary technical information |
| Mixpanel | Product usage and purchase flow analytics | Usage events, SDK identifiers, and necessary technical attributes |
| Email services | Feedback and contact you initiate | Email address, message, and attachments you send |
| GitHub Pages | Hosting the privacy policy website | Technical information needed for website visits and security logs |

This policy explains the purposes and scope of our use of these services in the app. Information provided by service providers does not replace our responsibility for the app's data processing.

Data may be processed outside your country or region. Mixpanel analytics requests currently use an EU regional endpoint; RevenueCat processing may involve infrastructure in the United States. Processing locations for Apple, GitHub, email, and other services also depend on their service arrangements. Using an EU endpoint does not mean all related service and support activities occur only in the EU.

For additional information about the providers' privacy practices:

- [Mixpanel Privacy Statement](https://mixpanel.com/legal/privacy-policy/)
- [RevenueCat Privacy Information](https://www.revenuecat.com/privacy)

## 9. Retention and deletion

### Local habits and check-in data

Relevant data is generally retained while you use the app until you delete it or the system removes the relevant app data.

You can delete an individual habit, including its related progress, events, and check-in photos.

You can also clear all check-in records for a particular habit while keeping the habit itself. Related progress, events, and photos are deleted, and related coin statistics are affected.

### iCloud data

If iCloud Sync is enabled when you delete data, the deletion propagates through Apple's synchronization mechanisms to the cloud and other devices. Deletion may take time to complete across locations and should not be understood as immediate removal everywhere.

Turning off synchronization or deleting the app does not actively remove previous iCloud data. You can manage relevant data through Apple's iCloud storage management tools.

### App removal, system backups, and other copies

When you delete the app, iOS handles local app-container data under its system rules. Removing the app is not the same as clearing synchronized cloud data, system backups, or copies you have saved elsewhere. iOS's Offload App option, which retains documents and data, can also have a different result from Delete App.

The current version does not provide a separate habit-data import, export, or manual backup feature. Apple's device and system backups are separate system mechanisms.

### Analytics, purchase, and feedback data

Deleting habits or removing the app does not automatically request deletion of historical data from Mixpanel, RevenueCat, or email services.

Relevant data is retained for the period needed for the analytics, membership processing, support, security, and other purposes described in this policy, taking into account legal obligations, dispute handling, and service deletion and backup mechanisms. The absence of an app account does not mean that analytics and purchase data does not exist.

You can request access or deletion through the contact email below. Where we can reliably associate your request with relevant records, we will handle data under our control and instruct service providers to assist where needed. The app has no registered accounts or in-app way to display your Mixpanel identifier. If we cannot reliably associate a request with particular analytics or purchase records, we will explain the practical limitations and cannot guarantee that every relevant record in third-party systems can be located and deleted. We cannot remotely access or delete content stored only on your device or in your personal iCloud private database on your behalf.

## 10. Your choices and rights

Using the app and iOS features, you can:

- View, edit, or delete habits, or clear check-in records for a particular habit;
- Change your nickname, avatar, and preferences;
- Enable or disable iCloud Sync and manage cloud data through Apple's tools;
- Adjust camera, photo, notification, and alarm permissions;
- Manage auto-renewing memberships through Apple's subscription management features;
- Contact us about this policy or related data under our control.

Depending on applicable law, you may also have rights to access, correction, deletion, copies, restriction of or objection to certain processing, and withdrawal of consent where applicable. Contact us using the email below to exercise applicable rights. We do not ask you to send your Apple Account password, banking details, or unnecessary habit journals or photos to identify a request.

## 11. Data security

We aim to minimize unnecessary data collection and transmission and separate core habit content from product and purchase analytics. Core data is primarily stored on your device and in Apple's private cloud environment when you choose to use it.

Devices, accounts, electronic storage, and network transmission cannot guarantee absolute security. Protect your device and Apple Account and adjust photo permissions and notification previews as appropriate.

## 12. Minors

If you are a minor, use the app with parental or guardian guidance or consent where required by applicable law. If you believe we have improperly processed a minor's personal information, contact us using the email below so we can investigate and act as required by law.

## 13. Changes to this policy

We may update this policy and its update date when features, data practices, or service use change. Where changes require additional notice or consent under applicable law, we will act accordingly.

## 14. Contact us

Operator / developer: QiHu Wang

Email: [qihu.studio@gmail.com](mailto:qihu.studio@gmail.com)

For privacy questions or data requests, please explain the feature involved and the type of request. We will respond within the period required by applicable law and verify requests only as necessary. If an extension is legally permitted and needed, we will explain the reason and next steps.
