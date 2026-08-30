### Plygon

Technical artist. Procedural systems and DCC tooling.

HOWEST DAE, Game Graphics Production. Working stack: Blender (`bpy`, Geometry Nodes, shader / compositor graphs), Houdini (SOP, VEX, HDAs), Python, Unreal PCG.

**[Plygon MCP](https://github.com/Plygonality/Plygon-mcp)** — flagship  
Local FastMCP bridges. Cursor speaks stdio; a DCC-side TCP listener runs commands on the main thread. Scene inspect → mutate → viewport capture → export. MIT. Bind is localhost only. No telemetry.

| DCC | Bind | Process |
|---|---|---|
| Blender 3.0+ | `127.0.0.1:9876` | add-on + `plygon-blender-mcp` |
| Houdini 19.5+ | `127.0.0.1:9877` | package + `plygon-houdini-mcp` |

The other public repos sit around that loop: graphs as data, a material system, a concept generator.

**[gn-as-code](https://github.com/Plygonality/gn-as-code)**  
Python API to build, dump, and diff Geometry Node trees as data. Git is the source of truth. The `.blend` is a cache. Plygon MCP applies a graph and screenshots the viewport.

**[HDA-as-code](https://github.com/Plygonality/HDA-as-code)**  
Same idea for Houdini SOP networks. Typed builders, canonical JSON, structural diffs. The `.hip` is a cache. Sibling of gn-as-code.

**[Master Node](https://github.com/Plygonality/Master-Node)**  
Blender N-panel that binds to a category master node and exposes its parameters. Framework public, presets paid. Artists look-dev in the viewport; they do not need Cursor.

**[Hard Sci-Fi Idea Generator](https://github.com/Plygonality/Hard-SciFi-idea-generator)**  
Hard sci-fi concept generator for 3D artists. Coherent megastructure prompts with lighting, palette, and composition notes.

[ArtStation](https://www.artstation.com/emil_van_dam) · [LinkedIn](https://www.linkedin.com/in/emil-van-dam-220731198) · [YouTube](https://youtube.com/@emiiiill20)
