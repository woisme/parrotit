# ParrotIt for setters

For businesses, charities and anyone who **sends** ParrotIt forms. Connect Claude to your ParrotIt account and ask about it in plain words:

- *"How did the open-day form do this week?"*
- *"When are the kiosks busiest?"*
- *"Which Keys haven't been used for a month?"*

## Install (Claude Code)

```
/plugin install parrotit-setter --marketplace woisme/parrotit
```

On Claude Code older than 2.1.275, use two lines instead:

```
/plugin marketplace add woisme/parrotit
/plugin install parrotit-setter
```

Then run `/mcp`, pick **parrotit-setter** and sign in. The ParrotIt approve page opens. Approve, and you're connected.

## Claude.ai and Claude Desktop

No plugin needed. Go to **Settings → Connectors → Add custom connector**, name it `ParrotIt` and paste:

```
https://parrotit.app/mcp
```

Then **Connect** and approve on ParrotIt. Grok and other AI apps use the same address. Your ParrotIt account shows the steps under **Integrations → AI connector**.

## What it can see

| | |
|---|---|
| Forms | Titles, questions, status, settings |
| Analytics | Opens, completion, responses by day, how people arrived, device type, returning responders. Field-level counts under 5 are hidden |
| Kiosks | Names, places on the map, when visits happen |
| Keys | Status, visits, visits per form, each Key's history |

**Never** what anyone wrote, who they are, or anything that is encrypted. ParrotIt checks every reply before it leaves.

It is **read only**. The one exception: it can write a *draft* form from a short brief, if you tick that when you connect. It can't publish, send or delete.

Every call is logged. Disconnect any time from **Integrations → AI connector** in ParrotIt.

## For people filling forms

That's the other plugin, [`parrotit`](../README.md): your AI fills forms from your own encrypted vault.
