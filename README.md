# [giscus][giscus]

A comments system powered by [GitHub Discussions][discussions]. Let visitors leave comments and reactions on your website via GitHub! Heavily inspired by [utterances][utterances].

- [Open source][repo]. 🌏
- No tracking, no ads, always free. 📡 🚫
- No database needed. All data is stored in GitHub Discussions. :octocat:
- GitHub themes: light, dark, dark dimmed, and more! 🌗
- Only ~40KB total chunks size. ⚡
- Automatically fetches new comments and edits from GitHub. 🔃
- Can be self-hosted! 🤳

> **Note:**\
> giscus is still under active development. GitHub is also still actively developing Discussions and its API. Thus, some features of giscus may break or change over time.

## how it works

When giscus loads, the [GitHub Discussions search API][search-api] is used to find the Discussion associated with the page based on a chosen mapping (URL, `pathname`, `<title>`, etc.). If a matching discussion cannot be found, the giscus bot will automatically create a discussion the first time someone leaves a comment or reaction.

To comment, visitors must authorize the [giscus app][giscus-app] to [post on their behalf][authorization] using the GitHub OAuth flow. Alternatively, visitors can comment on the GitHub Discussion directly. You can moderate the comments on GitHub.

[giscus]: https://giscus.app
[repo]: https://github.com/laymonage/giscus
[discussions]: https://docs.github.com/en/discussions
[utterances]: https://github.com/utterance/utterances
[search-api]: https://docs.github.com/en/graphql/guides/using-the-graphql-api-for-discussions#search
[giscus-app]: https://github.com/apps/giscus
[authorization]: https://docs.github.com/en/developers/apps/identifying-and-authorizing-users-for-github-apps

<!-- configuration -->

If you're using giscus, consider [starring 🌟 giscus on GitHub][repo] and adding the [`giscus`][giscus-topic] topic [to your repository][topic-howto]! 🎉

## migrating

If you've previously used other systems that utilize GitHub Issues (e.g. [utterances][utterances], [gitalk][gitalk]), you can [convert the existing issues into discussions][convert]. After the conversion, just make sure that the mapping between the discussion titles and the pages are correct, then giscus will automatically use the discussions.

## contributing

See [CONTRIBUTING.md][contributing]

[repo]: https://github.com/laymonage/giscus
[giscus-topic]: https://github.com/topics/giscus
[topic-howto]: https://docs.github.com/en/github/administering-a-repository/classifying-your-repository-with-topics
[utterances]: https://github.com/utterance/utterances
[gitalk]: https://github.com/gitalk/gitalk
[convert]: https://docs.github.com/en/discussions/managing-discussions-for-your-community/moderating-discussions#converting-an-issue-to-a-discussion
[contributing]: https://github.com/laymonage/giscus/blob/main/CONTRIBUTING.md
