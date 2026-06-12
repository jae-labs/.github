# Design Spec: jae-labs Profile README Redesign
**Date:** 2026-06-13
**Status:** Approved

## 1. Objective
Redesign the primary welcome landing page (`README.md`) for the `jae-labs` GitHub organization profile. 

The goal is to maintain the funny, cyberpunk "human agent" theme found on [justanother.engineer](https://justanother.engineer), but in a less visually flashy layout tailored to low-overhead markdown display.

## 2. Design Decisions
- **Tone:** Carbon-based biological SRE theme (`lui.z`).
- **Interactive Concept:** Mock terminal session using shell commands to title sections.
  - Section 1: `$` `cat /etc/motd` (Welcome greeting readout).
  - Section 2: `$` `who` (User log info: `lui.z         web      Jun  4 07:56`).
  - Section 3: `$` `uname` (Operating system name: `Darwin`).
  - Section 4: `$` `uptime` (Process uptime metadata tracking years since birth: `20:17  up 37 years, 1 user, load averages...`).
  - Section 5: `$` `tree` (Standard directory tree command output listing organization repositories, annotated with `#` comments explaining each).
  - Section 6: `$` `crontab -l` (Focus routines: sends wake-on-lan packet at 8:00 AM, creates a tmux session named `BUI` at 8:55 AM, launches a system root focus loop inside `BUI` running `make nice-things` at 9:00 AM, suspends focus loop and runs `make lunch` at 1:00 PM, resumes focus loop at 2:00 PM, suspends loop and stops active make jobs at 5:00 PM, and hibernates system at 11:00 PM).
- **Structure:** Removed arbitrary categories to deliver a flat list of items, aligning with the "bash style, no categories" user requirement. Removed footer, license, and memory blocks for maximum simplicity.
