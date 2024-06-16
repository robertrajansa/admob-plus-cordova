---
id: ad-request-options
title: Common Ad Request Options
sidebar_label: Ad Request Options
---

## Types

\<AUTOGENERATED_TABLE_OF_CONTENTS\>

## Reference

### `AdUnitIDOption`

```ts
type AdUnitIDOption =
  | string
  | {
      android: string;
      ios: string;
    };
```

### `IAdRequest`

```ts
interface IAdRequest {
  id?: AdUnitIDOption;
  testDevices?: string[];
  childDirected?: boolean;
  underAgeOfConsent?: boolean;
}
```

#### `id`

Ad unit ID.

Require to be a `string` or `{ android: string, ios: string }`.

#### `childDirected`

Child-directed setting.

Optional `boolean`.

Check out the official [Android](https://developers.google.com/admob/android/targeting#child-directed_setting) and [iOS](https://developers.google.com/admob/ios/targeting#child-directed_setting) doc for more info.

#### `testDevices`

Test device IDs.

Optional `string[]`.