# agents

<!--
Your tools, and what each one is allowed to see. In this plain-files template
the policy is enforced by YOU (you only paste/attach what's listed). In a
Level 1/2 implementation (see the USRKey format spec) this page becomes
machine-enforced policy, including what each tool may *propose* to change.

Format per tool:
  pages:     which of the six pages it gets
  writeback: none | propose | auto-accept   (per page)
-->

## claude-desktop
pages: identity, stack, now, history
writeback: propose (all granted)
<!-- My daily driver — gets the most context. -->

## cursor
pages: identity, stack, now
writeback: propose (now, stack); none (others)
<!-- Coding only. Doesn't need history. -->

## chatgpt-web
pages: identity, stack
writeback: none
<!-- Paste-card only; no MCP, no writeback. -->

## anything-else
pages: identity
writeback: none
<!-- Default for tools not listed: name and role, nothing more. -->
