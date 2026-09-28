# Digital Forensics Lab

Hands-on course repository for the digital forensics laboratory series — seven labs that walk students from the Linux command line all the way to memory forensics, using realistic artifacts and hidden flags.

All flags use the format `ctf{xxxx}`.

## Labs

| Lab | Topic | Materials |
| --- | --- | --- |
| [Lab 01](Lab%2001/) | Introduction to Digital Forensics — Linux CLI, hashing, magic bytes | Slides + working paper + 3 challenges |
| [Lab 02](Lab%2002/) | Common Windows Artifacts — registry, LNK, browsers, event logs | Slides + deep dive + working paper + 2 new challenges |
| [Lab 03](Lab%2003/) | Document Analysis and Steganography — OOXML, macros, stego | Slides + deep dive + working paper + 2 new challenges |
| [Lab 04](Lab%2004/) | Web Attack Forensics — Apache/ModSecurity logs | Upstream material |
| [Lab 05](Lab%2005/) | Network Traffic Forensics — Wireshark | Upstream material |
| [Lab 06](Lab%2006/) | Disk Image Forensics — FTK Imager, `$MFT` | Upstream material |
| [Lab 07](Lab%2007/) | Memory Forensics — Volatility | Upstream material |

Slides and working papers for Labs 2-7 follow the Lab 01 format as they are developed.

## Repository structure

```
Lab XX/
├── README.md                        # theory + instructions for the lab
├── files/                           # exercise artifacts (work on copies, never the originals)
├── instructor/                      # instructor-only references — do not distribute (Lab 01)
├── Lab XX Presentation.pptx / .pdf  # lecture deck (Lab 01)
└── Lab XX Working Paper.docx / .pdf # student worksheet to fill in and submit (Lab 01)
```

## Lab 01 at a glance

- **Presentation** — 17 slides: what digital forensics is, the digital trail, the twelve-command toolbox with live terminal examples, hashing for integrity, magic bytes, header repair, and the three challenges.
- **Working paper** — the worksheet students complete before, during, and after the session: pre-lab check, guided drills, challenges with staged hints, twelve analysis questions, reflection, and evidence/hash appendix forms.
- **Challenges** —
  - A: `files/challenge.png` — the original corrupted-header flag (from the upstream lab)
  - B: `files/challenge_extra.png` — a header that lies about its format
  - C: `files/access_big.log` + `update.bin` — an 8,600-line log hunt for grep, plus a binary for `strings`, with two hidden flags

## Credits

Based on the open lab series [aaltonen1024/digital-forensics-lab](https://github.com/aaltonen1024/digital-forensics-lab), extended with course challenges, slides, and working papers.
