# Git Sources

Git Sources defines where to fetch/pull your application code. 

These sources are used to:
- Setup helper apps (such as GitHub App, GitLab App) at your Git providers,
- Provides access through tokens/ssh keys to your repositories,
- Clone your application's code,
- Set up webhooks for automated deployments,
- etc...

## Types of supported Git Sources
Hosted or self-hosted versions of the following Git providers are supported:
- GitHub
- GitLab

## How to Integrate with Gitlab
1. (in Coolify) If you haven't already, in **Settings**, specify a URL (FQDN) like `coolify.yourdomain.com`. This is not required, but it makes the setup easier.
2. Once that's complete, close the page, navigate to `coolify.yourdomain.com`, and log back in
3. (in Coolify) In **Git Sources**, add a new GitLab source
4. In a new browser tab, navigate to your GitLab instance and find the UI to add a new application
5. (in GitLab) Enter the **Callback URL** as `https://coolify.yourdomain.com/webhooks/gitlab`
6. (in GitLab) check the following scopes: `api`, `read_repository`, `email`
7. (in GitLab) Save the application and copy the **Application ID** 
8. (in Coolify) In your new source, paste the **Application ID**
9. (in GitLab) In the newly created application, copy the **Secret**
10. (in Coolify) Paste the **Secret**
11. (in Coolify) Enter the OAuth ID. It will be the located at the end of the url of your GitLab application: https://yourgitlabdomain.com/oauth/applications/123456 👈
12. (in Coolify) Hit save
13. (in Coolify) In **Applications** add a new application with GitLab as the source
14. If you're still logged into GitLab, an authorization popup will appear. Click authorize.