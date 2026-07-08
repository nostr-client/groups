# groups

**Mailing lists on nostr.** Google-Groups-style communities read through a
Gmail-style three-pane UI — one buildless HTML file, no group server, no
signup.

**Live:** https://nostr-client.github.io/groups/

Built on [NIP-72](https://github.com/nostr-protocol/nips/blob/master/72.md)
communities (kind 34550) on ordinary public relays, so it's interoperable:
communities created in Satellite/Coracle/Amethyst show up in Discover, and
threads posted here show up there.

- **Discover** — recent community definitions from the relays
- **Your groups** — join/leave; persisted locally and published as your
  NIP-51 communities list (kind 10004) when logged in
- **Thread list** — Gmail rows: author, subject (NIP-14 `subject` tag or
  first line), snippet, reply count, age
- **Threads** — the shared [thread](https://github.com/nostr-client/thread)
  component: ancestors, live reply tree, reply box
- **New thread** — subject + body, tagged to the community
- deep links: `#34550:<pubkey>:<d>`

Phase 2 candidate: private encrypted lists (NIP-17 gift wrap) as a separate
repo. AGPL-3.0-or-later.
