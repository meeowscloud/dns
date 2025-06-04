# Meeows' DNS

[![test](https://github.com/meeowscloud/dns/workflows/test/badge.svg)](https://github.com/meeowscloud/dns/actions?query=workflow%3Atest)
[![deploy](https://github.com/meeowscloud/dns/workflows/deploy/badge.svg)](https://github.com/meeowscloud/dns/actions?query=workflow%3Adeploy)

This repository is used for managing Meeows' DNS configuration using [OctoDNS](https://github.com/octodns/octodns).

## Getting your own subdomain

Want your own meeows subdomain? Here's how you can get it:

1. **Fork this repo** - GitHub has a [great guide](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo) if you need help.
2. **Pick your domain** - We've got `meeows.net` and `meeows.cloud` available! Open the corresponding `.yaml` file (`meeows.net.yaml` or `meeows.cloud.yaml`) in your fork.

3. **Add your subdomain** - Find the right spot alphabetically (we like to keep things organized) and add something like this:

```yaml
your-cool-name:
  type: CNAME
  value: your-website.com.
```

**Quick setup guide:**

- Replace `your-cool-name` with whatever you want your subdomain to be (so `your-cool-name.meeows.net`)
- Replace `your-website.com.` with where you want it to point (don't forget that dot at the end!)
- Using an IP address instead? Change `type: CNAME` to `type: A`

4. **Commit and create a PR** - Save your changes, commit them, and [create a pull request](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request-from-a-fork)!

That's it! Someone will review your request and get you set up. 🎉

**Need to make changes?** Just update your fork and push the changes - no need to create a new PR!
