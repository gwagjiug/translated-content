---
title: "Permissions-Policy: midi"
slug: Web/HTTP/Reference/Headers/Permissions-Policy/midi
original_slug: Web/HTTP/Headers/Permissions-Policy/midi
---

{{HTTPSidebar}}{{SeeCompatTable}}

HTTP の {{HTTPHeader("Permissions-Policy")}} ヘッダーにおける `midi` ディレクティブは、現在の文書が [Web MIDI API](/ja/docs/Web/API/Web_MIDI_API) を使用することを許可するかどうかを制御します。このポリシーが有効であれば、 {{domxref("Navigator.requestMIDIAccess()")}} から返却された {{jsxref("Promise")}} が `DOMException` で拒否されます。

## 構文

```
Permissions-Policy: midi <allowlist>;
```

- \<allowlist>
  - : この機能を許可するオリジンのリストです。 [`Permissions-Policy`](/ja/docs/Web/HTTP/Reference/Headers/Permissions-Policy#%E6%A7%8B%E6%96%87) を参照してください。

## 既定のポリシー

許可リストは `'self'` です。

## 仕様書

{{Specifications}}

## ブラウザーの互換性

{{Compat}}

## 関連情報

- {{HTTPHeader("Permissions-Policy")}} ヘッダー
- [機能ポリシー](/ja/docs/Web/HTTP/Guides/Permissions_Policy)
- [機能ポリシーの使用](/ja/docs/Web/HTTP/Guides/Feature_Policy/Using_Feature_Policy)
