# Google Ads skills

Twelve Google Ads skills vendored into this repository so Claude Code picks them
up automatically in any session (local CLI, desktop, or web) without needing the
interactive `/plugin` command, which is unavailable in remote/web sessions.

| Skill | Focus |
| --- | --- |
| `google-ads-audit` | Full account audit and health check |
| `keyword-research` | Keyword discovery, match types, negatives |
| `ad-copy-generation` | RSA headlines, descriptions, assets |
| `budget-optimization` | Budget allocation and bidding strategy |
| `pmax-optimization` | Performance Max asset groups and signals |
| `shopping-ads` | Shopping campaigns and Merchant Center feeds |
| `audience-targeting` | Audience segments and targeting layers |
| `conversion-tracking` | Conversion setup, values, attribution |
| `quality-score-optimization` | Relevance, CTR, landing page experience |
| `remarketing-strategy` | Remarketing lists and sequencing |
| `competitor-analysis` | Auction insights and competitive gaps |
| `landing-page-audit` | Post-click experience and conversion rate |

`shopping-ads` is the most directly relevant to this repository: it covers
Merchant Center product feed attributes, title optimization, custom labels, and
supplemental feeds — the same ground as `orozyme_ua_feed.xml`.

## Source

Vendored from [itallstartedwithaidea/agent-skills](https://github.com/itallstartedwithaidea/agent-skills)
(marketplace `googleadsagent-skills`, plugin `google-ads-skills`) by
googleadsagent.ai, at commit `7a04ccbde5f96d4bfe99a15a7e6fd96a7a4d4cd6`.

Licensed MIT 丑 see `LICENSE.upstream`.

## Updating

```sh
git clone --depth 1 https://github.com/itallstartedwithaidea/agent-skills.git /tmp/agent-skills
cp -r /tmp/agent-skills/skills/google-ads/* .claude/skills/
cp /tmp/agent-skills/LICENSE .claude/skills/LICENSE.upstream
```

Then refresh the commit hash recorded above.
