# Talha Ahmed

**I make asset pipelines survive their own scale.**

Sixteen years of pipeline and tools engineering for animation and VFX studios, with engine-side
integration through Unreal Interchange. Most recently core developer and architect of Epic's
Megascans to OpenUSD conversion.

## The last eighteen months

At Epic I built and operated the pipeline that converted **20,637 assets**, roughly 92 percent of the
complete Megascans library, into self-contained **USDZ and MaterialX** packages on open standards.

- **Two interchangeable backends, one API.** A Houdini engine with five custom HDAs driven in `hython`,
  and a pure Python backend with a vendored USD runtime and no DCC dependency. I drove the native
  backend to structural parity with the Houdini one.
- **An independent QA gate, roughly 110 rules across seven layers.** It re-derived its expectations
  from its own constants and never imported the converter, so a wrong backend could not pass its own
  output. Both had to clear the same gate.
- **Rule first, then fix.** Every defect reported by an artist became a new rule and a permanent
  regression test, which is why the gate got sharper over eighteen months rather than looser.
- **Corpus scale operations.** More than thirty asset classes identified by structure and type,
  corruption detection, an auditable rejection path, idempotent relaunch, and 98.9 percent coverage of
  the mandated asset list.

## What I work on

- OpenUSD, MaterialX and OpenPBR, from conversion through validation and packaging
- Maya and Houdini APIs, with Qt and PySide interfaces for the people who use them
- Asset models and metadata that stay upright on decade-old production data
- Build and release automation for content, not only for code
- Colour management, per-map colour space, and the unglamorous parts of image fidelity

## Reading

The engineering behind those bullets is written up rather than summarised.

- **[Megascans to OpenUSD, the series](https://magicreddeer.github.io/blog)**. Six posts on the dual
  backends, the QA gate, the FBX reader that preserves pivots a standard import flattens, the provider
  model for bad metadata, the colour and displacement rules, and keeping a twenty thousand asset run
  alive.
- **[Nebula Pipeline Toolbox documentation](https://nebula-pipeline-toolbox-docs.readthedocs.io/en/master/)**.
  A departmentalized Maya and Redshift pipeline I designed and documented, from production planning
  through lighting, rendering and post.

## Earlier work

At ICE Animations the studio published its Maya tooling openly under EPL 2.0. Five of those repositories
carry most of my commits, and each carries a copyright notice in my name:

- **[mocapToRig](https://github.com/iceanimations/mocapToRig)**. HumanIK retargeting from motion capture
  skeletons onto control rigs.
- **[multishot](https://github.com/iceanimations/multishot)**. Sequence preview and cache export from
  animation scenes in Maya.
- **[mvstereo](https://github.com/iceanimations/mvstereo)**. A stereo camera rig in Maya.
- **[ICEDBQueries](https://github.com/iceanimations/ICEDBQueries)**. The SQL behind the studio's
  production and attendance tracking.
- **[PipelineTooBoxManual](https://github.com/iceanimations/PipelineTooBoxManual)**. The written manual
  for the departmental pipeline toolbox.

Ten of those repositories are mirrored to this account with their full history, because a link only
shows that code exists and a mirror lets it be read. Each README states what the tool does and who wrote
which part. Six of the ten, chiefly `loader`, `createShots`, `expoCache` and `bakeInstancer`, are the work
of Qurban Ali from my team, and their READMEs say so in the first paragraph rather than leaving it to be
found in the commit graph.

The **Nebula Pipeline**, a modular production pipeline I designed and led from 2019 to 2021 with a small
team, is published module by module on
[Bitbucket](https://bitbucket.org/nebulapipeline/workspace/repositories), with
[documentation on Read the Docs](https://nebula-pipeline-toolbox-docs.readthedocs.io/en/master/). It
integrates with Southpaw's TACTIC for asset management and uses Marcus Ottosson's Qt.py for binding
compatibility; neither of those is my work, and the
[architecture index](https://github.com/MagicRedDeer/nebula-pipeline) says so explicitly.

## Elsewhere

Portfolio · [magicreddeer.github.io](https://magicreddeer.github.io)
Resume · [Pipeline and tools](https://magicreddeer.github.io/resume/Talha_Ahmed_Resume_PipelineTD.pdf)
LinkedIn · [talha-ahmed-lazyleopard](https://www.linkedin.com/in/talha-ahmed-lazyleopard)
Email · [talha.ahmed@gmail.com](mailto:talha.ahmed@gmail.com)

Available for contract and full-time work. Remote from Karachi, async across UK, EU and Asia hours, and
I invoice through my own company when a studio would rather not run payroll in Pakistan.
