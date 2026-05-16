## Minghou Lei · 李明皓

**Game Engine R&D Engineer · 游戏引擎研发工程师**  
[Kingsoft · Amazing Seasun Games](https://www.amazingseasun.com/) · Engine Platform · Commercial Engine Team  
西山居 · 引擎平台 · 商业引擎组 · 广东珠海

> *Building rendering systems that hold up under production pressure — carefully, curiously, and with a bit of stubbornness.*
>
> *用严谨的工程方法处理复杂的渲染问题——认真、好奇，以及一点点执着。*

---

### About · 关于

Game engine engineer at [Amazing Seasun Games](https://www.amazingseasun.com/) (Kingsoft) since 2021, on the **Engine Platform · Commercial Engine Team**. Most of my time goes into customizing **Unity** at the engine level to ship rendering capabilities Unity doesn't give you out of the box — distributed voxel GI baking, Nanite-like virtual geometry, OIT hair, hierarchical lighting topology. I also do **Xbox / PS5 platform debugging** to keep cross-platform parity sane. The JX3 project still uses our in-house engine **KG3DEngine**, so I work across both.

入职西山居（金山）**引擎平台·商业引擎组** 至今,主力基于 **Unity 引擎深度定制** 为多款产品提供渲染底层——在 Unity 上自研落地体素 GI 烘焙、类 Nanite 虚拟几何体、OIT 毛发、多主角分层光照等非原生能力,同时负责 **Xbox / PS5 主机平台渲染调试** 保证多端一致性；JX3 项目使用自研引擎 **KG3DEngine**。

I care about graphics debuggers that tell the truth, tools that reduce guesswork, and rendering code that clearly explains what it is doing. Side track: bringing AI coding agents into large-scale engine codebases.

关心说真话的图形调试器、减少猜测的工具,以及能清楚表达自身行为的渲染代码。副线探索 AI 辅助引擎研发工作流。

---

### Shipped Titles · 参与项目

| Game · 游戏 | Stack · 技术栈 | Contribution · 参与方向 |
|---|---|---|
| [**Mecha BREAK · 解限机**](https://store.steampowered.com/app/2452280/) | Unity · PC / Xbox / PS5 | OIT hair · distributed voxel GI baking · Nanite-like virtual geometry pipeline · hierarchical multi-actor lighting · SSR / SSGI · **console platform debugging** |
| [**Starsand Island · 星砂岛**](https://store.steampowered.com/app/2966320/) | Unity · PC / Switch 2 / Xbox | Static/dynamic shadow split · GPU skinning at scale · foliage interaction system |
| [**JX3 · 剑网3**](https://jx3.xoyo.com) | KG3DEngine · 自研 | Editor-side lighting debug tooling — perf statistics panel, debug toggles (Cluster Debug compatible), in-editor heatmap overlay |
| **Me and My Cat · 我和我的猫** | Unity · 项目终止 | Point light real-time shadows · SSAO · light probe optimization |

---

### Focus Areas · 技术方向

| Area · 方向 | Details · 具体内容 |
|---|---|
| Real-time Rendering · 实时渲染 | Deferred shading, multi-pass lighting, **Unity SRP deep customization** |
| Lighting & GI · 光照与全局光照 | Voxel-based distributed GI baking, hierarchical lighting topology, light probe optimization |
| Console Platforms · 主机平台 | **Xbox / PS5** rendering debugging, cross-platform parity & stability |
| Streaming & Virtual Geometry · 流式渲染 | Nanite-like virtual geometry, LOD streaming, cache-backed fallback, peak memory control |
| Hair Rendering · 毛发渲染 | OIT transparency blending, depth-ordered compositing |
| Graphics Tooling · 图形调试工具链 | RenderDoc / PIX / native console GPU profilers, editor-side diagnostic tools |
| AI Engineering · AI 工程化 | Coding agents, context engineering, cross-engine migration via AI tooling |

---

### Research & Patents · 研究与专利

I'm credited on **8 invention patents** in game engine rendering — **4 as first inventor**, **2 already granted**, and **6 shipped in production** (Mecha BREAK, Me and My Cat).

发明专利 **8 项**——**第一发明人 4 项**,**已授权 2 项**；**6 项已落地至量产项目**（解限机、我和我的猫）。

Coverage: hierarchical lighting topology · LOD-based streaming · adaptive cross-platform rendering · OIT hair · voxel-based distributed baking · probe optimization · regional lighting.

方向：分层/拓扑光照计算 · LOD 流式渲染 · 多端自适配 · OIT 毛发透明混合 · 体素化分布式烘焙 · 探针优化 · 区域光照。

<details>
<summary><b>First-inventor patents · 第一发明人专利（4 项）</b></summary>
<br>

| Patent No. | Topic | Shipped In |
|---|---|---|
| **CN119215405A** (2024) | OIT hair multi-fragment transparency blending | Mecha BREAK · hair rendering |
| **CN121074231A** (2025) | Hierarchical lighting topology by object priority | Mecha BREAK · multi-actor lighting |
| **CN117218273A** (2023) | Voxel-based distributed GI baking | Mecha BREAK · open-world GI |
| **CN115487495A / B** ✓ granted (2025) | Environment lighting × light-source ratio compositing | Prototype validation |

</details>

---

### AI Engineering · AI 工程化探索

Side-time exploration on bringing AI coding agents into large-scale game engine development.

工作之余系统性探索 AI 辅助引擎研发在大规模引擎代码库下的落地路径。

- **OSS contributions** — merged PRs to multi-thousand-star AI coding agent projects, focused on Codex hook stability and session continuity
- **Personal-led project** — built a **JX3 → UE5 cross-engine migration pipeline** via AI tooling, with **AI texture enhancement (NVIDIA NVTT3 / DLISR)**; completed end-to-end demo on two scenes
- **Benchmarked impact** — measured **−78% shell calls / −20% token usage** on the KG3DEngine codebase, adopted by 5–8 colleagues as daily workflow
- **Local inference stack** — Mac Mini M1 (16GB) running MLX + Qwen3-9B-4bit, serving the Windows dev machine across the LAN

- **开源贡献** — 在头部 AI Coding Agent 开源项目（万星级）有 PR 被合并的贡献记录
- **个人主导项目** — 主导 **剑网3 → UE5 跨引擎迁移工具链路**,含 **NVIDIA NVTT3 / DLISR AI 贴图增强**；完成两个场景的端到端迁移演示
- **量化效果** — 在 KG3DEngine 代码库实测 **Shell 调用 −78% / Token −20%**,推动团队 5–8 人采纳为日常工作流
- **本地推理栈** — Mac Mini M1（16GB）运行 MLX + Qwen3-9B-4bit,为 Windows 开发机供能

Internal speaker at the company's TA bootcamp.

担任公司内部 TA 训练营技术分享讲师。

---

### Tech Stack · 技术栈

**Languages · 语言**

![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=csharp&logoColor=white)
![HLSL](https://img.shields.io/badge/HLSL-5C2D91?style=flat-square&logoColor=white)
![ShaderLab](https://img.shields.io/badge/ShaderLab-000000?style=flat-square&logo=unity&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=flat-square&logo=powershell&logoColor=white)

**Engine / Rendering · 引擎与渲染**

![Unity](https://img.shields.io/badge/Unity-000000?style=flat-square&logo=unity&logoColor=white)
![KG3DEngine](https://img.shields.io/badge/KG3DEngine-8B0000?style=flat-square&logoColor=white)
![Unreal Engine](https://img.shields.io/badge/Unreal%20Engine-313131?style=flat-square&logo=unrealengine&logoColor=white)
![DirectX 11](https://img.shields.io/badge/DirectX%2011-0078D4?style=flat-square&logoColor=white)
![RenderDoc](https://img.shields.io/badge/RenderDoc-CC3333?style=flat-square&logoColor=white)
![NVIDIA Nsight](https://img.shields.io/badge/NVIDIA%20Nsight-76B900?style=flat-square&logo=nvidia&logoColor=white)

**Console Platforms · 主机平台**

![PlayStation 5](https://img.shields.io/badge/PlayStation%205-003791?style=flat-square&logo=playstation5&logoColor=white)
![Xbox](https://img.shields.io/badge/Xbox-107C10?style=flat-square&logo=xbox&logoColor=white)
![Nintendo Switch 2](https://img.shields.io/badge/Switch%202-E60012?style=flat-square&logo=nintendoswitch&logoColor=white)

**IDE / AI Tooling · 开发与 AI 工具**

![Rider](https://img.shields.io/badge/Rider-000000?style=flat-square&logo=rider&logoColor=white)
![Visual Studio](https://img.shields.io/badge/Visual%20Studio-5C2D91?style=flat-square&logo=visualstudio&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)
![PyCharm](https://img.shields.io/badge/PyCharm-000000?style=flat-square&logo=pycharm&logoColor=white)
![Claude Code](https://img.shields.io/badge/Claude%20Code-D97757?style=flat-square&logo=claude&logoColor=white)
![Codex](https://img.shields.io/badge/Codex-111111?style=flat-square&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=flat-square&logoColor=white)
![MLX](https://img.shields.io/badge/MLX-000000?style=flat-square&logo=apple&logoColor=white)

---

### Featured Repositories · 精选公开仓库

A handful of graphics demos worth a look:

- [**GPU-Skinning-Demo**](https://github.com/Minghou-Lei/GPU-Skinning-Demo) — GPU Skinning × GPU Instancing showcase · ⭐ 137
- [**Realtime-point-light-shadows-in-unity-URP**](https://github.com/Minghou-Lei/Realtime-point-light-shadows-in-unity-URP) — Real-time point light shadows for Unity 2020 URP · ⭐ 51
- [**Light-Probe-Demo**](https://github.com/Minghou-Lei/Light-Probe-Demo) — Light probe technical notes · ⭐ 16
- [**unity-texture-debugger**](https://github.com/Minghou-Lei/unity-texture-debugger) — Runtime texture display for GBuffer / AO textures · ⭐ 14
- [**SSAO-Demo**](https://github.com/Minghou-Lei/SSAO-Demo) — Screen Space Ambient Occlusion implementation · ⭐ 10

---

### GitHub Activity · 统计

<div align="center">

<img height="160" src="https://github-readme-stats.vercel.app/api?username=Minghou-Lei&show_icons=true&theme=radical&hide_border=true&cache_seconds=86400" />
&nbsp;
<img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Minghou-Lei&layout=compact&theme=radical&hide_border=true&langs_count=6&cache_seconds=86400" />

</div>

---

### Contact · 联系

[GitHub](https://github.com/Minghou-Lei) &nbsp;·&nbsp; [LinkedIn](https://www.linkedin.com/in/%E6%98%8E%E7%9A%93-%E6%9D%8E-597356105/) &nbsp;·&nbsp; [脉脉](https://maimai.cn/contact/share/card?u=kgmsdwiqpe9a&_share_channel=copy_link) &nbsp;·&nbsp; [Instagram](https://www.instagram.com/mistletoer76/)

<img src="https://komarev.com/ghpvc/?username=Minghou-Lei&style=flat-square&color=555555&label=views" alt="Profile views" />

---

<details>
<summary>⏱ WakaTime Coding Stats · 编码统计</summary>
<br>

<!--START_SECTION:waka-->
![Code Time](http://img.shields.io/badge/Code%20Time-656%20hrs%2026%20mins-blue)

```text
💬 Languages this week:
C#                       8 hrs 52 mins       ██████████████████████░░░   88.85 %
HLSL                     51 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   08.59 %
ShaderLab                8 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.40 %
Csproj                   3 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.52 %

🔥 Editor: Rider  |  💻 OS: Windows  |  🕑 Asia/Shanghai
```

<!--END_SECTION:waka-->

</details>
