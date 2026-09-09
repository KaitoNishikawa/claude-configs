# Global preferences

- Write a docstring for every function you create (and add one when editing a function that lacks it). 
- **Always modify files with the Edit / Write / NotebookEdit tools — never via Bash (`sed -i`, heredocs, `python - <<EOF`, `cat >`, `tee`, `mv`/`cp` over existing files, etc.).** This applies even in auto mode, which otherwise asks you to prefer Bash: `/rewind` checkpoints only track the dedicated file tools, so Bash-side edits can't be undone. Bash is fine for reading, searching, running scripts, and git.
- When the user is describing a problem, asking a question, or thinking out loud rather than requesting a change, the deliverable is your assessment. Report your findings/thoughts and stop. Don't apply a fix until they ask for one.