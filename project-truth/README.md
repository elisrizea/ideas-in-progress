# Project Truth: a Shazam for video claims

**Idea · design draft** · Alin Rizea, DBM AI · October 2026

**Read it:** https://elisrizea.github.io/ideas-in-progress/project-truth/
· [PDF](project-truth.pdf)

## The idea

Many misleading clips are real footage, cut so that someone seems to say what they did not mean. Project Truth
ingests source footage ahead of time (interviews, debates, news, speeches), transcribes it, extracts every factual
claim with speaker, timestamp and topic, and stores audio, visual and transcript fingerprints for every few seconds.

Share a clip to the Project Truth app from TikTok, Instagram, Facebook, X, YouTube or WhatsApp, and it:

- finds the original footage, even if the clip was cropped, re-encoded or re-captioned;
- shows what was really said around it and flags what was cut, with timestamps;
- lists every claim in the clip, what is wrong with each one, and a confidence rating based on the evidence found;
- links to the same claim in other videos;
- processes the clip on the spot if it is not in the archive yet, and adds it, so the next check is instant.

Nothing is built yet. The paper covers the design, the hard parts (coverage, deepfakes, rights, biometrics,
defamation) and how I would test it.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The design draft (self-contained, served by GitHub Pages) |
| `project-truth.pdf` | The same document as an A4 PDF |
| `cover.png` | Link-preview card |

I'm looking for a newsroom or fact-checking team, people who have worked on video copy detection or audio
fingerprinting, misinformation researchers, and funding. See the [main page](../) for how to get in touch.
