---
layout: default
title: Account & Data Deletion
permalink: /account-deletion/
---

# AutoBud — Account & Data Deletion

_Last updated: May 22, 2026_

This page explains how to request deletion of your **AutoBud** account (Customer App or Mechanic App) and the data associated with it. It applies to both `AutoBud` (customers) and `AutoBud Tech` (mechanics), which share a single account system.

## How to request deletion

We do not yet offer an in-app "Delete my account" button. To request deletion, email us from the address associated with your AutoBud account:

- **Email:** [vshashankrao@gmail.com](mailto:vshashankrao@gmail.com)
- **Subject:** `Delete my AutoBud account`
- **Include:** the email address you sign in with, and which app you use (AutoBud customer, AutoBud Tech, or both).

We respond within **3 business days** to confirm the request and complete deletion within **30 days**.

If you cannot email us from the address on the account (for example, because you signed up with "Sign in with Apple" using a private relay email you no longer have access to), include enough information for us to identify the account — your name as it appears in the app, the approximate sign-up date, and the last job or quote you remember.

## What is deleted

When we process your request, we permanently delete:

- Your **profile** (name, avatar, contact details, and — for Mechanics — business name, bio, portfolio photos, service area).
- Your **vehicles** (make, model, year, VIN) if you are a Customer.
- All **jobs you posted**, including their titles, descriptions, photos, and ZIP-level location data.
- All **quotes you sent or received** that are not tied to a completed or in-progress booking.
- All **chat messages** you sent or received.
- All **push notification device tokens** registered to your account.
- Your **avatar and portfolio photos** stored in our object storage.
- Your **authentication record** (the Supabase Auth user), which removes your ability to sign in with email/password, Apple, or Google.

## What is retained, and for how long

We retain a limited set of records after deletion when we are legally or operationally required to:

- **Completed bookings and the quotes that produced them** are retained for up to **90 days** for tax, dispute-resolution, and refund purposes. These records are stripped of your profile (your name is replaced with "Deleted user") but retain the booking date, price, and scope so the other party's transaction history remains intact. After 90 days they are permanently deleted.
- **Reviews you wrote about a Mechanic** are retained but anonymized — your name is replaced with "Deleted user". The other party's reputation history is preserved.
- **Crash reports and performance telemetry** sent to Sentry are retained for **90 days** under Sentry's standard retention. These reports do not include the contents of your messages, posts, or profile; they include only a Sentry-generated installation ID, device model, OS version, and stack trace.
- **Backups.** Our database provider (Supabase) takes encrypted point-in-time backups. Your data may persist in those backups for up to **30 days** after deletion before being rotated out. Backups are not used for any purpose other than disaster recovery.

## If you only want to delete *some* of your data

You don't need to delete your whole account to remove specific items:

- **Delete a posted job** that hasn't been booked: open the job in the app and tap **Delete**.
- **Remove a booked / completed job from your list:** open the job and tap **Remove** (this hides it from your view; the underlying booking record is retained for the other party).
- **Delete a vehicle from your garage:** Profile → Vehicles → swipe / tap delete on the vehicle.
- **Remove your avatar or portfolio photos:** Profile → Edit profile.
- **Stop notifications:** revoke notification permission in iOS or Android system settings.

If you would like a specific item deleted that isn't covered above, email the same address with the details.

## Contact

Questions about this policy or about a deletion request:

- **Email:** [vshashankrao@gmail.com](mailto:vshashankrao@gmail.com)

See also our [Privacy Policy](./privacy) and [Terms and Conditions](./terms).
