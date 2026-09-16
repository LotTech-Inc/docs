# LotTech customer help

## Audience and scope

- Write for dealership customers: managers and rooftop admins.
- A rooftop means one dealership location. Both roles are limited to their assigned rooftops.
- Managers handle daily work within assigned product roles and manage their own preferences.
- Rooftop admins also manage their dealership's team and shared configuration.
- Never treat LotTech's internal Administrator role as a customer role or direct readers to platform-wide Admin pages.
- Do not document employee-only provisioning, global user management, rooftop creation, channel activation, or internal implementation details. Direct customer requests for those changes to LotTech support.

## Content evidence

- Verify steps, button labels, and access rules in the dashboard source before publishing. Source: `../lottech-voice-website/lottech-voice-frontend` and its backend sibling.
- Do not infer rooftop-admin capabilities from the internal `isAdmin` branch. Check the actual permission controlling each action.
- Use **Invite Teammate** for new team access. Do not tell rooftop admins to create accounts with another person's password.
- Personal notification and transfer preferences are the same preferences whether changed from Settings or by a rooftop admin from Team.
- Describe only verified customer behavior. Avoid guarantees about call answering, delivery, timing, or future features.

## Writing and publishing

- This site uses Mintlify. Pages are MDX with title and description frontmatter; navigation lives in `docs.json`.
- Use the Mintlify skill for components and validation.
- Write in second person, use concise instructions, and bold exact UI labels.
- Say "rooftop admin" instead of the ambiguous "admin". Use department manager labels where they clarify the workflow.
- Keep manager tasks easy to find. Put shared configuration and team-management instructions under Rooftop admins.
- Keep documentation changes focused on user workflows, not source files or backend mechanics.
- Run `mint broken-links` and `mint validate`, and inspect the rendered preview before publishing.
- Remove employee-only pages from published content; hiding them from navigation alone is insufficient. Redirect retired links to the relevant customer guide.
