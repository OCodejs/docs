### Code of Conduct

- [x] I have read and agree to the GitHub Docs project's [Code of Conduct](https://github.com/github/docs/blob/main/.github/CODE_OF_CONDUCT.md)

### What article on docs.github.com is affected?

https://docs.github.com/en/billing/concepts/product-billing/github-packages#free-use-of-github-packages

### What part(s) of the article would you like to see updated?

> **Billing for container image storage:** _Container image storage_ and bandwidth _for the Container registry is currently free_. If you use Container registry, you'll be informed at least one month in advance of any change to this policy. For more information about the Container registry, see [Working with the Container registry](https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-container-registry).

### Additional information

1. I'm in an organization (not an enterprise) on a team plan
2. In that organization is a repository with a ghcr package
3. Only one workflow generates classic github workflow artifacts and they're tiny and have a fairly short expiration (so they can't accumulate month over month)
4. One workflow generates ghcr images labeled with the repository
5. There is no garbage collection configured for this repository for the ghcr side (obviously, we will be adding it)

I checked the billing history for April and October.

### April

```csv
"date","product","sku","quantity","unit_type","applied_cost_per_quantity","gross_amount","discount_amount","net_amount","username","organization","repository","workflow_path","cost_center_name"
"date","product","sku","quantity","unit_type","applied_cost_per_quantity","gross_amount","discount_amount","net_amount","username","organization","repository","workflow_path","cost_center_name"
"2026-04-01","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-04-02","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-04-03","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-04-04","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-04-05","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-04-06","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-04-07","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-04-08","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-04-09","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-04-10","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-04-11","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-04-12","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-04-13","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-04-14","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-04-15","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-04-16","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","","Organization","repository","",""
"2026-04-17","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-04-18","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-04-19","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-04-20","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-04-21","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-04-22","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-04-23","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-04-24","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-04-25","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-04-26","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-04-27","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-04-28","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-04-29","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-04-30","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
```

### October

```csv
"date","product","sku","quantity","unit_type","applied_cost_per_quantity","gross_amount","discount_amount","net_amount","username","organization","repository","workflow_path","cost_center_name"
"2026-10-01","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-10-02","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-10-03","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-10-04","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-10-05","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-10-06","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-10-07","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-10-08","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-10-09","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-10-10","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-10-11","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-10-12","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","0          ","","Organization","repository","",""
"2026-10-13","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","xxxxxxxxxxx","","Organization","repository","",""
"2026-10-14","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-10-15","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-10-16","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-10-17","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-10-18","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-10-19","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-10-20","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-10-21","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-10-22","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-10-23","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-10-24","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-10-25","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-10-26","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-10-27","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-10-28","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-10-29","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-10-30","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
"2026-10-31","actions","actions_storage","xxxxxxxxxxx","gigabyte-hours","xxxxxxxxxx","xxxxxxxxxxx","0          ","xxxxxxxxxxx","","Organization","repository","",""
```

This repository is clearly becoming more expensive over time, and the cost is almost certainly because of the ghcr.io hosted packages. Which contradicts the naive reading of the quoted text and all the ai hallucinations derived from that text.

I'm willing to believe that github is not currently charging for _bandwidth_ -- I certainly don't see any records in my billing records for this repository (we're billed for actions_storage and actions_linux* minutes).

---

This appears to be the official beta announcement (September 1, 2020; Updated June 18, 2021):
[Introducing GitHub Container Registry](https://github.blog/news-insights/product-news/introducing-github-container-registry/)

> Our users have asked for anonymous access for public container images, similar to how we enable anonymous access to public repositories of source code today. Anonymous access is available with GitHub Container Registry today, and we’ve gotten things started today by publishing a [public image](https://github.com/orgs/github/packages/container/super-linter) of our [own super-linter](https://github.blog/2020-06-18-introducing-github-super-linter-one-linter-to-rule-them-all/). **GitHub Container Registry is free for public images**. _Container Registry is free for private images during the beta_, and _as part of GitHub Packages will follow the same pricing model when generally available_.

And the GA announcement (June 21, 2021; Updated December 19, 2021):

[GitHub Packages Container registry is generally available](https://github.blog/news-insights/product-news/github-packages-container-registry-generally-available/)

> At this time, usage of the Container registry will continue to be free. Billing for Container registry usage will begin in the coming months with ample notice as to when that change will occur. Container registry pricing for storage and bandwidth will follow the standard GitHub Packages [pricing structure](https://github.com/features/packages#pricing).
