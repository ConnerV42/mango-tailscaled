# mango-tailscaled

A small `tailscaled` build for a GL.iNet Mango router (linux/mipsle, softfloat). It is Tailscale v1.104.4 with most features removed. It keeps the kernel-TUN subnet router and the CLI. Size: 15.7 MB, 5.2 MB gzipped.

The router has no room for it in flash. After each boot, it downloads `tailscaled.gz` from the release and checks the sha256 before it runs the file.

| File | sha256 |
|---|---|
| `tailscaled` | `41f064b9466d15d1eba1a769be6c28559b608f01858486fd7ddeb31540cfaaf2` |
| `tailscaled.gz` | `3b7bbebf0ff7713a6b8d1cd8ff45e159f38ab51ae785768fca3d5ca3d290df1f` |

- Source: [tailscale/tailscale v1.104.4](https://github.com/tailscale/tailscale/tree/v1.104.4). Build: [`build.sh`](build.sh) (Go 1.27.3).
- License: BSD-3-Clause, Copyright (c) 2020 Tailscale Inc & contributors. See [LICENSE](LICENSE).
