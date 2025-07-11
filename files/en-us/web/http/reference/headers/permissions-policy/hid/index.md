---
title: "Permissions-Policy: hid directive"
short-title: hid
slug: Web/HTTP/Reference/Headers/Permissions-Policy/hid
page-type: http-permissions-policy-directive
status:
  - experimental
browser-compat: http.headers.Permissions-Policy.hid
sidebar: http
---

{{SeeCompatTable}}

The HTTP {{HTTPHeader("Permissions-Policy")}} header `hid` directive controls whether the current document is allowed to use the {{domxref("WebHID API", "WebHID API", "", "nocode")}} to connect to uncommon or exotic human interface devices such as alternative keyboards or gamepads.

Specifically, where a defined policy blocks WebHID usage, the {{domxref("Navigator.hid")}} property will not be available.

## Syntax

```http
Permissions-Policy: hid=<allowlist>;
```

- `<allowlist>`
  - : A list of origins for which permission is granted to use the feature. See [`Permissions-Policy` > Syntax](/en-US/docs/Web/HTTP/Reference/Headers/Permissions-Policy#syntax) for more details.

## Default policy

The default allowlist for `hid` is `self`.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- {{HTTPHeader("Permissions-Policy")}} header
- [Permissions Policy](/en-US/docs/Web/HTTP/Guides/Permissions_Policy)
