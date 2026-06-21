# parrotit (plugin)

The ParrotIt plugin for Claude Code. It bundles the ParrotIt MCP connector
(`@parrotit/mcp-responder`) so your AI can read from and save to your encrypted
ParrotIt vault on demand — decrypted only on your own machine, every action
logged and revocable.

**Install:**

```
/plugin marketplace add woisme/parrotit
/plugin install parrotit
```

Then pair your device once:

```
npx -y @parrotit/mcp-responder pair
```

…and approve it in the ParrotIt app under **My Devices**.

Full documentation, the trust boundary, and what the AI can read or save:
see the [repository README](../README.md).
