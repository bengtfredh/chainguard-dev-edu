---
date: 2023-04-10T21:58:49Z
title: "chainctl auth identities view"
slug: chainctl_auth_identities_view
url: /chainguard/chainguard-enforce/chainctl-docs/chainctl_auth_identities_view/
draft: false
tags: ["chainctl", "Reference", "Product"]
images: []
type: "article"
toc: true
---
## chainctl auth identities view

View the details of an identity.

```
chainctl auth identities view {IDENTITY_NAME | IDENTITY_ID} [flags]
```

### Options

```
  -h, --help   help for view
```

### Options inherited from parent commands

```
      --api string                   The url of the Chainguard platform API. (default "http://api.api-system.svc")
      --audience string              The Chainguard token audience to request. (default "http://api.api-system.svc")
      --config string                A specific chainctl config file.
      --console string               The url of the Chainguard platform Console. (default "http://console-ui.api-system.svc")
      --issuer string                The url of the Chainguard STS endpoint. (default "http://issuer.oidc-system.svc")
  -o, --output string                Output format. One of: ["", "table", "tree", "json", "id", "wide"]
      --timestamp-authority string   The url of the Chainguard Timestamp Authority endpoint. (default "http://tsa.timestamp-authority.svc")
  -v, --v int                        Set the log verbosity level.
```

### SEE ALSO

* [chainctl auth identities](/chainguard/chainguard-enforce/chainctl-docs/chainctl_auth_identities/)	 - Identity management.
