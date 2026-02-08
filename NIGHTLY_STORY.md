# Nightly Story Workflow

This document captures the routine for the 22:00 (Asia/Shanghai) story drop.

1. **Time**: Run after 22:00 Asia/Shanghai every day.
2. **File naming**: `stories/YYYY-MM-DD-<slug>.md` where `<slug>` is 2-3 lowercase English words joined with hyphens describing the tone.
3. **Front matter**:
   - First line: `# <Chinese Title>`
   - Second line: `YYYY-MM-DD`
   - Blank line, then 5-8 short paragraphs (Chinese prose, ~250-400 Chinese characters total).
   - End with `---` and `_故事：傻妞_`.
4. **README**: Insert a Markdown bullet at the top of the stories list linking to the new file.
5. **Git**:
   - Worktree: `/home/botclaw/workspacebot/story-tales`
   - Commands: `git pull --rebase`, add new file + README, commit `feat: nightly story YYYY-MM-DD`, push to `origin master`.
6. **Delivery**: After push, send the full story (or a short intro + link) back to老板 in the main session.
