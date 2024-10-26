# alfred-antidote-12-workflow

Permet d’accéder aux ressoures d’Antidote 12

## Changelog

Based on Jolin Masson’s Antidote 11 workflow (https://www.packal.org/workflow/antidote-11), I replaced `AgentAntidoteConnect` with `ServiceConnectixAntidote` in every `osascript` script.

For example, the original script

```
tell application "AgentAntidoteConnect"
	launch module dictionaries resource definitions word "{query}"
end tell
```

becomes

```
tell application "ServiceConnectixAntidote"
	launch module dictionaries resource definitions word "{query}"
end tell
```

