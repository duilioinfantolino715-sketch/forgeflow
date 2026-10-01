<!-- LOVABLE:BEGIN -->
> [!IMPORTANT]
> This project is connected to [Lovable](https://lovable.dev). Avoid rewriting
> published git history — force pushing, or rebasing/amending/squashing commits
> that are already pushed — as it rewrites history on Lovable's side and the
> user will likely lose their project history.
>
> Commits you push to the connected branch sync back to Lovable and show up in
> the editor, so keep the branch in a working state.
<!-- LOVABLE:END -->

## Project architecture

- Reuse `ForgeflowLogo` for branded navigation surfaces so the confirmed logo remains consistent across the app.
- Reuse `DashboardSidebar` across authenticated workspace pages so primary navigation remains consistent.
- Billing uses Lovable built-in Stripe embedded checkout; webhook syncs subscriptions table and profiles.subscription_status.
- Keep the authenticated Atelier as a separate workspace route; the existing project dashboard remains available from it.
