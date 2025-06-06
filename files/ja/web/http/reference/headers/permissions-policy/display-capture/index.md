---
title: "Permissions-Policy: display-capture"
slug: Web/HTTP/Reference/Headers/Permissions-Policy/display-capture
original_slug: Web/HTTP/Headers/Permissions-Policy/display-capture
---

{{HTTPSidebar}} {{SeeCompatTable}}

HTTP の {{HTTPHeader("Permissions-Policy")}} ヘッダーにおける `display-capture` ディレクティブは、現在の文書が [Screen Capture API](/ja/docs/Web/API/Screen_Capture_API)、すなわち {{domxref("MediaDevices.getDisplayMedia", "getDisplayMedia()")}} を使用して画面の内容をキャプチャすることを許可するかどうかを制御します。

文書で `display-capture` が無効になっていた場合、文書は {{domxref("MediaDevices.getDisplayMedia", "getDisplayMedia()")}} を通じて画面キャプチャを行うことができなくなります。

## 構文

```
Permissions-Policy: display-capture <allowlist>;
```

- \<allowlist>
  - : この機能を許可するオリジンのリストです。 [`Permissions-Policy`](/ja/docs/Web/HTTP/Reference/Headers/Permissions-Policy#%E6%A7%8B%E6%96%87) を参照してください。

## 既定のポリシー

`display-capture` の許可リストの既定値は `'self'` です。

## 仕様書

{{Specifications}}

## ブラウザーの互換性

{{Compat}}

## 関連情報

- {{HTTPHeader("Permissions-Policy")}} ヘッダー
- [機能ポリシー](/ja/docs/Web/HTTP/Guides/Permissions_Policy)
- [機能ポリシーの使用](/ja/docs/Web/HTTP/Guides/Feature_Policy/Using_Feature_Policy)
- [Screen Capture API](/ja/docs/Web/API/Screen_Capture_API)
- [Screen Capture API の使用](/ja/docs/Web/API/Screen_Capture_API/Using_Screen_Capture)
