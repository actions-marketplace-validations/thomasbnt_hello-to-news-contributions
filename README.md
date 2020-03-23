# 👋 **Hello to news contributors**

##### Hey to first PR and Issues for news contributors. Customize your message, add links to Guidelines or other importants files.


[![License](https://img.shields.io/github/license/thomasbnt/hello-to-news-contributions.svg?style=for-the-badge)](https://github.com/thomasbnt/hello-to-news-contributions/blob/master/LICENSE)
[![Support me on BMC](https://img.shields.io/badge/Support-Buy%20Me%20A%20Coffee-orange.svg?style=for-the-badge)](https://www.buymeacoffee.com/thomasbnt)
____

Create the `.github/workflows/hello-tonews-contributions.yml` file with the following configuration

```yml
name: Auto message for PR's and Issues
description: Automatically send hello message to the first PR and Issue for new contributor.
branding:
  icon: message-square
  color: yellow
on: [pull_request, issues]
jobs:
  build:
    name: Hello new contributor
    runs-on: ubuntu-latest
    steps:
      - uses: actions/first-interaction@v1
        with:
          repo-token: ${{ secrets.GITHUB_TOKEN }}
          issue-message: "Hey, thank you for opening your first Issue ! 🙂"
          pr-message: "Hey, thank you for opening your Pull Request !"
```

- 📣  News : Follow me on [Twitter](https://twitter.com/Hyprimort)
- 🔗  See my [website](https://thomasbnt.fr) !
- 📨  [Send me a email !](https://thomasbnt.fr/contact)

![Love Open Source](https://badges.frapsoft.com/os/v3/open-source.png?v=103)
