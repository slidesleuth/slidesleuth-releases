# SlideSleuth MCPB — supplemental documentation

SlideSleuth allows compatible agents to find timestamped visual and spoken
evidence in YouTube videos through a local MCP (currently only Apple-silicon
supported). The MCP connects Claude Desktop to the locally installed
SlideSleuth Desktop app; it is not a remote server, hosted endpoint, Docker
deployment, or Glama deployment.

This page supplements the existing `README.md` and the published release
assets. It does not replace or modify the README, the `v0.2.9` release tag, or
the downloadable DMG and MCPB files.

## Download

- [SlideSleuth 0.2.9 MCPB](https://github.com/slidesleuth/slidesleuth-releases/releases/download/v0.2.9/SlideSleuth-0.2.9.mcpb)
- [SlideSleuth 0.2.9 DMG and MCPB release](https://github.com/slidesleuth/slidesleuth-releases/releases/tag/v0.2.9)

MCPB SHA-256:

`eee95e33402991881ed66479fb361fbfac9d3b8f4979488132c85a98ded5b8db`

## Install

Follow the instructions at [SlideSleuth MCP setup guide](https://www.slidesleuth.com/agent-access/)

## Review prompt (paste in Claude chat after SlideSleuth Desktop and MCP install)

"Use SlideSleuth to find slides about batteries in https://www.youtube.com/watch?v=LUFJE5QkINg and explain each slide."

## Expected result

- Claude should display a widget including a gallery of slides from the video
  relating to the prompt request.
- Clicking on a slide should show it in the larger viewing window along with
  its accompanying explanatory text.
- The **View in SlideSleuth** link should bring the SlideSleuth Desktop app to
  the foreground and show the selected slide within the visual list of all the
  found slides in the video.

## Scope and limits

- SlideSleuth currently supports YouTube videos only.
- The local MCP currently supports Apple-silicon macOS only.
- Slide discovery and analysis depends on the presentation of visual data
  inside each video and the user’s subscription tier. Visual Slide Focus and
  Topic Focus require Plus or Pro access.
- Spoken Text depends on supported English captions.
- Results may include errors or omissions; check the original video when
  accuracy matters.
- The public browser demo is open to all visitors and lets them explore example
  video analyses: <https://www.slidesleuth.com/demo>

## Disclosure

SlideSleuth Desktop and MCP is our work.

## Privacy and support

- [Privacy Policy](https://www.slidesleuth.com/privacy/)
- [Support](https://www.slidesleuth.com/contact/)
- [Agent setup](https://www.slidesleuth.com/agent-access/)

Directory-specific source, licensing, and manifest requirements are separate
from this documentation page. Creating this page does not alter the published
`v0.2.9` MCPB or make any claim that the release package is a remote MCP.
