---
date: 2023-04-10T21:58:49Z
title: "chainctl auth identities delete"
slug: chainctl_auth_identities_delete
url: /chainguard/chainguard-enforce/chainctl-docs/chainctl_auth_identities_delete/
draft: false
tags: ["chainctl", "Reference", "Product"]
images: []
type: "article"
toc: true
---
## chainctl auth identities delete

Delete an identity.

```
chainctl auth identities delete {IDENTITY_NAME | IDENTITY_ID} [--yes] [--output ] [flags]
```

### Options

```
  -h, --help   help for delete
  -y, --yes    Automatic yes to prompts; assume "yes" as answer to all prompts and run non-interactively.
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
