---
name: rk-handoff
description: Create a development handoff document for Rockchip SDK development, including current status, modified files, verification results, remaining issues and next debugging steps.
argument-hint: "Describe what the next session should focus on"
---

You are preparing a handoff document for another AI agent.

The goal is NOT to summarize the conversation.

The goal IS to allow another engineer or AI agent to immediately continue development without rereading the entire conversation.

Generate a Markdown document with the following structure.

---

# Goal

Describe the overall objective in one or two sentences.

---

# Background

Summarize only the information that is necessary to understand the task.

Do not repeat unnecessary discussion.

---

# Current Status

List what has already been completed.

For every completed item explain:

- what was done
- why it was done
- whether it has been verified

---

# Modified Files

List every modified file.

For each file include:

- path
- purpose
- important functions or structures changed

Example:

kernel-6.1/drivers/media/platform/rockchip/rkcif.c

- add BT1120 support
- modify media bus format
- add debug logs

---

# Build Commands

List every command required to reproduce the build.

Example:

./build.sh lunch

./build.sh bmake:camera-engine-rkaiq-rebuild

---

# Verification Commands

Include every command used for debugging.

Examples:

media-ctl

v4l2-ctl

modetest

gst-launch

cat /sys/...

dmesg

grep

---

# Current Problem

Describe exactly what is still wrong.

Include

Expected Result

Actual Result

Observed Logs

---

# Root Cause Analysis

List:

Confirmed causes

Ruled-out causes

Possible causes

Confidence level for each.

---

# Next Recommended Steps

Provide a prioritized checklist.

Example

1. Verify DTS
2. Verify media graph
3. Dump registers
4. Check ISP routing
5. Compare with RK3588 implementation

---

# Important References

List only important references.

For example

source files

documents

datasheets

commits

previous discussions

Do NOT duplicate long content.

---

# Suggested Skills

Recommend which skills should be invoked next.

Examples

/debug

/grill-me

/tdd

/git

---

# Notes

Record any temporary conclusions that should not be forgotten.

Avoid recording unnecessary conversation history.

If the user provided an argument when invoking this skill, tailor the handoff toward that future task.