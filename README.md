# Obsidian Diagrams.Net

A plugin for [Obsidian](https://obsidian.md/) for inserting and editing [diagrams.net](https://diagrams.net/) (previously draw.io) diagrams.

Based on [obsidian-diagrams-net](https://github.com/jensmtg/obsidian-diagrams-net) by Jens M Gleditsch; modified by [BalSla](https://github.com/BalSla). See [LICENSE](./LICENSE) for the original copyright notice and MIT license.

## Releases and alternative plugin manager

Push a tag matching the version in `manifest.json` (for example `v1.1.0` or `1.1.0`), or run the **Create Release** workflow manually. Manual runs use `v` followed by the manifest version. The workflow builds the plugin and publishes `main.js`, `manifest.json`, and `LICENSE`; this plugin has no `styles.css`.

We recommend using the alternative plugin manager to install and manage updates for this plugin. Add a plugin with repository URL `https://github.com/BalSla/obsidian-diagrams-net` and plugin folder `obsidian-diagrams-net`. The manager checks the latest published release and requires a manual plugin reload after an update.

> ## ⚠️ **Caveats**
> As Obsidian itself has an API that is under development, so is this plugin. There are some things you should be aware of if you are using it:
> 
> - Diagrams are saved as a separate file – ``MyDiagram.svg.xml``, alongside their image representation – ``MyDiagram.svg``. (The .xml-file can be opened directly in any diagrams.net-editor.)
> - Moving and renaming a diagram inside Obsidian will do so for both the diagram file and the image file. However, since there is no "copy" event to listen to in the Obsidian API, copying a diagram means the new diagram will not have a diagram file associated with it, and as such, cannot be opened in the editor.
> - The workaround, if you need to copy a diagram, is to manually duplicate and rename both the image and diagram file.

> ## 🐛 **Known issues**
> - Editing a diagram will not update the image in the active editor, you need to force a reload or navigate away and back to see the updates.

