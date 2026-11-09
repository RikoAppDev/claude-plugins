# Claude Code plugins

Claude Code plugins and mods by RikoAppDev, in one marketplace. Each plugin lives in its own repository; this one only lists them.

Skills are kept apart, in [RikoAppDev/skills](https://github.com/RikoAppDev/skills), so that other agents can use them too.

## Plugins

| Plugin | Kind | What it does |
| --- | --- | --- |
| [loose-ends](https://github.com/RikoAppDev/loose-ends) | mod | Keeps the questions and tasks Claude left for you, word for word, in a panel beside the chat |

## Install

At the prompt of a Claude Code terminal session, add this marketplace once, then install any plugin from it:

```
/plugin marketplace add RikoAppDev/claude-plugins
/plugin install <plugin>@rikoappdev-plugins
```

From a shell:

```
claude plugin marketplace add RikoAppDev/claude-plugins
claude plugin install <plugin>@rikoappdev-plugins
```

## Adding a plugin

1. Give the plugin its own repository with a `.claude-plugin/plugin.json`.
2. List it in `.claude-plugin/marketplace.json`:

   ```json
   {
     "name": "<plugin>",
     "description": "<one line>",
     "source": { "source": "github", "repo": "RikoAppDev/<repo>" }
   }
   ```

3. Check the marketplace with `claude plugin validate .`.
4. Add the plugin to the table above.

## License

[MIT](LICENSE)
