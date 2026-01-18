
<div align="center">
  <img src="https://res.cloudinary.com/anuraghazra/image/upload/v1594908242/logo_ccswme.svg" width="100px" alt="GitHub Readme Stats" />
  <h1 style="font-size: 28px; margin: 10px 0;">GitHub Readme Stats</h1>
  <p>Get dynamically generated GitHub stats on your READMEs!</p>
</div>

<p align="center">
  <a href="https://github.com/anuraghazra/github-readme-stats/actions">
    <img alt="Tests Passing" src="https://github.com/anuraghazra/github-readme-stats/workflows/Test/badge.svg" />
  </a>
  <a href="https://github.com/anuraghazra/github-readme-stats/graphs/contributors">
    <img alt="GitHub Contributors" src="https://img.shields.io/github/contributors/anuraghazra/github-readme-stats" />
  </a>
  <a href="https://codecov.io/gh/anuraghazra/github-readme-stats">
    <img alt="Tests Coverage" src="https://codecov.io/gh/anuraghazra/github-readme-stats/branch/master/graph/badge.svg" />
  </a>
  <a href="https://github.com/anuraghazra/github-readme-stats/issues">
    <img alt="Issues" src="https://img.shields.io/github/issues/anuraghazra/github-readme-stats?color=0088ff" />
  </a>
  <a href="https://github.com/anuraghazra/github-readme-stats/pulls">
    <img alt="GitHub pull requests" src="https://img.shields.io/github/issues-pr/anuraghazra/github-readme-stats?color=0088ff" />
  </a>
  <br />
  <br />
  <a href="https://vercel.com?utm_source=github_readme_stats_team&utm_campaign=oss">
    <img src="./powered-by-vercel.svg"/>
  </a>
</p>

<p align="center">
  <a href="#all-demos">View Demo</a>
  ·
  <a href="https://github.com/anuraghazra/github-readme-stats/issues/new?assignees=&labels=bug&projects=&template=bug_report.yml">Report Bug</a>
  ·
  <a href="https://github.com/anuraghazra/github-readme-stats/issues/new?assignees=&labels=enhancement&projects=&template=feature_request.yml">Request Feature</a>
  ·
  <a href="https://github.com/anuraghazra/github-readme-stats/discussions/1770">FAQ</a>
  ·
  <a href="https://github.com/anuraghazra/github-readme-stats/discussions/new?category=q-a">Ask Question</a>
</p>

<p align="center">Love the project? Please consider <a href="https://www.paypal.me/anuraghazra">donating</a> to help the original author improve it!</p>

<details>
<summary>Table of contents (Click to show)</summary>

- [GitHub Stats Card](#github-stats-card)
    - [Hiding individual stats](#hiding-individual-stats)
    - [Showing additional individual stats](#showing-additional-individual-stats)
    - [Showing icons](#showing-icons)
    - [Showing commits count for specified year](#showing-commits-count-for-specified-year)
    - [Themes](#themes)
    - [Customization](#customization)
- [GitHub Extra Pins](#github-extra-pins)
    - [Usage](#usage)
    - [Options](#options)
    - [Demo](#demo)
- [GitHub Gist Pins](#github-gist-pins)
    - [Usage](#usage-1)
    - [Options](#options-1)
    - [Demo](#demo-1)
- [Top Languages Card](#top-languages-card)
    - [Usage](#usage-2)
    - [Options](#options-2)
    - [Language stats algorithm](#language-stats-algorithm)
    - [Exclude individual repositories](#exclude-individual-repositories)
    - [Hide individual languages](#hide-individual-languages)
    - [Show more languages](#show-more-languages)
    - [Compact Language Card Layout](#compact-language-card-layout)
    - [Donut Chart Language Card Layout](#donut-chart-language-card-layout)
    - [Donut Vertical Chart Language Card Layout](#donut-vertical-chart-language-card-layout)
    - [Pie Chart Language Card Layout](#pie-chart-language-card-layout)
    - [Hide Progress Bars](#hide-progress-bars)
    - [Change format of language's stats](#change-format-of-languages-stats)
    - [Demo](#demo-2)
- [WakaTime Stats Card](#wakatime-stats-card)
    - [Options](#options-3)
    - [Demo](#demo-3)
- [All Demos](#all-demos)
  - [Quick Tip (Align The Cards)](#quick-tip-align-the-cards)
    - [Stats and top languages cards](#stats-and-top-languages-cards)
    - [Pinning repositories](#pinning-repositories)
- [Deploy on your own](#deploy-on-your-own)
  - [First step: get your Personal Access Token (PAT)](#first-step-get-your-personal-access-token-pat)
    - [Classic token](#classic-token)
    - [Fine-grained token](#fine-grained-token)
  - [On Vercel](#on-vercel)
  - [On other platforms](#on-other-platforms)
  - [Available environment variables](#available-environment-variables)
  - [Keep your fork up to date](#keep-your-fork-up-to-date)
- [:sparkling_heart: Support the project](#sparkling_heart-support-the-project)
</details>

# Important Notices > [!NOTE]
> This is a self-hosted instance running on **frigg-stats.vercel.app**.

# GitHub Stats Card

Copy and paste this into your markdown, and that's it. Simple!

Change the `?username=` value to your GitHub username.

```md
[![Frigg's GitHub stats](https://frigg-stats.vercel.app/api?username=Frigg1337)](https://github.com/Frigg1337)

```

> [!NOTE]
> Available ranks are S (top 1%), A+ (12.5%), A (25%), A- (37.5%), B+ (50%), B (62.5%), B- (75%), C+ (87.5%) and C (everyone).

### Hiding individual stats

You can pass a query parameter `&hide=` to hide any specific stats with comma-separated values.

> Options: `&hide=stars,commits,prs,issues,contribs`

```md
![Frigg's GitHub stats](https://frigg-stats.vercel.app/api?username=Frigg1337&hide=contribs,prs)

```

### Showing additional individual stats

You can pass a query parameter `&show=` to show any specific additional stats with comma-separated values.

> Options: `&show=reviews,discussions_started,discussions_answered,prs_merged,prs_merged_percentage`

```md
![Frigg's GitHub stats](https://frigg-stats.vercel.app/api?username=Frigg1337&show=reviews,discussions_started,discussions_answered,prs_merged,prs_merged_percentage)

```

### Showing icons

To enable icons, you can pass `&show_icons=true` in the query param, like so:

```md
![Frigg's GitHub stats](https://frigg-stats.vercel.app/api?username=Frigg1337&show_icons=true)

```

### Showing commits count for specified year

You can specify a year and fetch only the commits that were made in that year by passing `&commits_year=YYYY` to the parameter.

```md
![Frigg's GitHub stats](https://frigg-stats.vercel.app/api?username=Frigg1337&commits_year=2024)

```

### Themes

With inbuilt themes, you can customize the look of the card without doing any [manual customization](https://www.google.com/search?q=%23customization).

Use `&theme=THEME_NAME` parameter like so :

```md
![Frigg's GitHub stats](https://frigg-stats.vercel.app/api?username=Frigg1337&show_icons=true&theme=radical)

```

#### All inbuilt themes

GitHub Readme Stats comes with several built-in themes (e.g. `dark`, `radical`, `merko`, `gruvbox`, `tokyonight`, `onedark`, `cobalt`, `synthwave`, `highcontrast`, `dracula`).

<img src="https://res.cloudinary.com/anuraghazra/image/upload/v1595174536/grs-themes_l4ynja.png" alt="GitHub Readme Stats Themes" width="600px"/>

You can look at a preview for [all available themes](https://www.google.com/search?q=themes/README.md) or checkout the [theme config file](https://www.google.com/search?q=themes/index.js).

#### Responsive Card Theme

##### Use the transparent theme

We have included a `transparent` theme that has a transparent background. This theme is optimized to look good on GitHub's dark and light default themes. You can enable this theme using the `&theme=transparent` parameter like so:

```md
![Frigg's GitHub stats](https://frigg-stats.vercel.app/api?username=Frigg1337&show_icons=true&theme=transparent)

```

<details>
<summary>:eyes: Show example</summary>

</details>

##### Add transparent alpha channel to a themes bg_color

You can use the `bg_color` parameter to make any of [the available themes](https://www.google.com/search?q=themes/README.md) transparent. This is done by setting the `bg_color` to a color with a transparent alpha channel (i.e. `bg_color=00000000`):

```md
![Frigg's GitHub stats](https://frigg-stats.vercel.app/api?username=Frigg1337&show_icons=true&bg_color=00000000)

```

<details>
<summary>:eyes: Show example</summary>

</details>

### Customization

You can customize the appearance of all your cards however you wish with URL parameters.

#### Common Options

| Name | Description | Type | Default value |
| --- | --- | --- | --- |
| `title_color` | Card's title color. | string (hex color) | `2f80ed` |
| `text_color` | Body text color. | string (hex color) | `434d58` |
| `icon_color` | Icons color if available. | string (hex color) | `4c71f2` |
| `border_color` | Card's border color. Does not apply when `hide_border` is enabled. | string (hex color) | `e4e2e2` |
| `bg_color` | Card's background color. | string (hex color or a gradient in the form of *angle,start,end*) | `fffefe` |
| `hide_border` | Hides the card's border. | boolean | `false` |
| `theme` | Name of the theme, choose from [all available themes](https://www.google.com/search?q=themes/README.md). | enum | `default` |
| `cache_seconds` | Sets the cache header manually (min: 21600, max: 86400). | integer | `21600` |
| `locale` | Sets the language in the card, you can check full list of available locales [here](https://www.google.com/search?q=%23available-locales). | enum | `en` |
| `border_radius` | Corner rounding on the card. | number | `4.5` |

#### Stats Card Exclusive Options

| Name | Description | Type | Default value |
| --- | --- | --- | --- |
| `hide` | Hides the [specified items](https://www.google.com/search?q=%23hiding-individual-stats) from stats. | string (comma-separated values) | `null` |
| `hide_title` | Hides the title of your stats card. | boolean | `false` |
| `card_width` | Sets the card's width manually. | number | `500px  (approx.)` |
| `hide_rank` | Hides the rank and automatically resizes the card width. | boolean | `false` |
| `rank_icon` | Shows alternative rank icon (i.e. `github`, `percentile` or `default`). | enum | `default` |
| `show_icons` | Shows icons near all stats. | boolean | `false` |
| `include_all_commits` | Count total commits instead of just the current year commits. | boolean | `false` |
| `line_height` | Sets the line height between text. | integer | `25` |
| `exclude_repo` | Excludes specified repositories. | string (comma-separated values) | `null` |
| `custom_title` | Sets a custom title for the card. | string | `<username> GitHub Stats` |
| `text_bold` | Uses bold text. | boolean | `true` |
| `disable_animations` | Disables all animations in the card. | boolean | `false` |
| `ring_color` | Color of the rank circle. | string (hex color) | `2f80ed` |
| `number_format` | Switches between two available formats for displaying the card values `short` (i.e. `6.6k`) and `long` (i.e. `6626`). | enum | `short` |
| `number_precision` | Enforce the number of digits after the decimal point for `short` number format. Must be an integer between 0 and 2. Will be ignored for `long` number format. | integer (0, 1 or 2) | `null` |
| `show` | Shows [additional items](https://www.google.com/search?q=%23showing-additional-individual-stats) on stats card (i.e. `reviews`, `discussions_started`, `discussions_answered`, `prs_merged` or `prs_merged_percentage`). | string (comma-separated values) | `null` |
| `commits_year` | Filters and counts only commits made in the specified year. | integer *(YYYY)* | `<current year> (one year to date)` |

---

# GitHub Extra Pins

GitHub extra pins allow you to pin more than 6 repositories in your profile using a GitHub readme profile.

### Usage

Copy-paste this code into your readme and change the links.

Endpoint: `api/pin?username=Frigg1337&repo=ctf-event-tracker`

```md
[![Readme Card](https://frigg-stats.vercel.app/api/pin/?username=Frigg1337&repo=ctf-event-tracker)](https://github.com/Frigg1337/ctf-event-tracker)

```

### Options

You can customize the appearance and behavior of the pinned repository card using the [common options](https://www.google.com/search?q=%23common-options) and exclusive options listed in the table below.

| Name | Description | Type | Default value |
| --- | --- | --- | --- |
| `show_owner` | Shows the repo's owner name. | boolean | `false` |
| `description_lines_count` | Manually set the number of lines for the description. Specified value will be clamped between 1 and 3. | number | `null` |

### Demo

Use `show_owner` query option to include the repo's owner username

# GitHub Gist Pins

GitHub gist pins allow you to pin gists in your GitHub profile using a GitHub readme profile.

### Usage

Copy-paste this code into your readme and change the links.

Endpoint: `api/gist?id=bbfce31e0217a3689c8d961a356cb10d`

```md
[![Gist Card](https://frigg-stats.vercel.app/api/gist?id=bbfce31e0217a3689c8d961a356cb10d)](https://gist.github.com/Yizack/bbfce31e0217a3689c8d961a356cb10d/)

```

# Top Languages Card

The top languages card shows a GitHub user's most frequently used languages.

### Usage

Copy-paste this code into your readme and change the links.

Endpoint: `api/top-langs?username=Frigg1337`

```md
[![Top Langs](https://frigg-stats.vercel.app/api/top-langs/?username=Frigg1337)](https://github.com/Frigg1337)

```

### Options

You can customize the appearance and behavior of the top languages card using the [common options](https://www.google.com/search?q=%23common-options) and exclusive options listed in the table below.

| Name | Description | Type | Default value |
| --- | --- | --- | --- |
| `hide` | Hides the [specified languages](https://www.google.com/search?q=%23hide-individual-languages) from card. | string (comma-separated values) | `null` |
| `hide_title` | Hides the title of your card. | boolean | `false` |
| `layout` | Switches between five available layouts `normal` & `compact` & `donut` & `donut-vertical` & `pie`. | enum | `normal` |
| `card_width` | Sets the card's width manually. | number | `300` |
| `langs_count` | Shows more languages on the card, between 1-20. | integer | `5` for `normal` and `donut`, `6` for other layouts |
| `exclude_repo` | Excludes specified repositories. | string (comma-separated values) | `null` |
| `custom_title` | Sets a custom title for the card. | string | `Most Used Languages` |
| `disable_animations` | Disables all animations in the card. | boolean | `false` |
| `hide_progress` | Uses the compact layout option, hides percentages, and removes the bars. | boolean | `false` |
| `size_weight` | Configures language stats algorithm (see [Language stats algorithm](https://www.google.com/search?q=%23language-stats-algorithm)). | integer | `1` |
| `count_weight` | Configures language stats algorithm (see [Language stats algorithm](https://www.google.com/search?q=%23language-stats-algorithm)). | integer | `0` |
| `stats_format` | Switches between two available formats for language's stats `percentages` and `bytes`. | enum | `percentages` |

### Language stats algorithm

We use the following algorithm to calculate the languages percentages on the language card:

```js
ranking_index = (byte_count ^ size_weight) * (repo_count ^ count_weight)

```

By default, only the byte count is used for determining the languages percentages shown on the language card (i.e. `size_weight=1` and `count_weight=0`).

* `&size_weight=1&count_weight=0` - *(default)* Orders by byte count.
* `&size_weight=0.5&count_weight=0.5` - *(recommended)* Uses both byte and repo count for ranking
* `&size_weight=0&count_weight=1` - Orders by repo count

```md
![Top Langs](https://frigg-stats.vercel.app/api/top-langs/?username=Frigg1337&size_weight=0.5&count_weight=0.5)

```

### Exclude individual repositories

You can use the `&exclude_repo=repo1,repo2` parameter to exclude individual repositories.

```md
![Top Langs](https://frigg-stats.vercel.app/api/top-langs/?username=Frigg1337&exclude_repo=github-readme-stats,anuraghazra.github.io)

```

### Hide individual languages

You can use `&hide=language1,language2` parameter to hide individual languages.

```md
![Top Langs](https://frigg-stats.vercel.app/api/top-langs/?username=Frigg1337&hide=javascript,html)

```

### Show more languages

You can use the `&langs_count=` option to increase or decrease the number of languages shown on the card. Valid values are integers between 1 and 20 (inclusive). By default it was set to `5` for `normal` & `donut` and `6` for other layouts.

```md
![Top Langs](https://frigg-stats.vercel.app/api/top-langs/?username=Frigg1337&langs_count=8)

```

### Compact Language Card Layout

You can use the `&layout=compact` option to change the card design.

```md
![Top Langs](https://frigg-stats.vercel.app/api/top-langs/?username=Frigg1337&layout=compact)

```

### Donut Chart Language Card Layout

You can use the `&layout=donut` option to change the card design.

```md
[![Top Langs](https://frigg-stats.vercel.app/api/top-langs/?username=Frigg1337&layout=donut)](https://github.com/Frigg1337)

```

### Donut Vertical Chart Language Card Layout

You can use the `&layout=donut-vertical` option to change the card design.

```md
[![Top Langs](https://frigg-stats.vercel.app/api/top-langs/?username=Frigg1337&layout=donut-vertical)](https://github.com/Frigg1337)

```

### Pie Chart Language Card Layout

You can use the `&layout=pie` option to change the card design.

```md
[![Top Langs](https://frigg-stats.vercel.app/api/top-langs/?username=Frigg1337&layout=pie)](https://github.com/Frigg1337)

```

### Hide Progress Bars

You can use the `&hide_progress=true` option to hide the percentages and the progress bars (layout will be automatically set to `compact`).

```md
![Top Langs](https://frigg-stats.vercel.app/api/top-langs/?username=Frigg1337&hide_progress=true)

```

### Change format of language's stats

You can use the `&stats_format=bytes` option to display the stats in bytes instead of percentage.

```md
![Top Langs](https://frigg-stats.vercel.app/api/top-langs/?username=Frigg1337&stats_format=bytes)

```

### Demo

* Compact layout
* Donut Chart layout

* Donut Vertical Chart layout

* Pie Chart layout

* Hidden progress bars
* Display bytes instead of percentage

# WakaTime Stats Card

Change the `?username=` value to your [WakaTime](https://wakatime.com) username.

```md
[![Frigg's WakaTime stats](https://frigg-stats.vercel.app/api/wakatime?username=Frigg1337)](https://github.com/Frigg1337)

```

### Options

You can customize the appearance and behavior of the WakaTime stats card using the [common options](https://www.google.com/search?q=%23common-options) and exclusive options listed in the table below.

| Name | Description | Type | Default value |
| --- | --- | --- | --- |
| `hide` | Hides the languages specified from the card. | string (comma-separated values) | `null` |
| `hide_title` | Hides the title of your card. | boolean | `false` |
| `card_width` | Sets the card's width manually. | number | `495` |
| `line_height` | Sets the line height between text. | integer | `25` |
| `hide_progress` | Hides the progress bar and percentage. | boolean | `false` |
| `custom_title` | Sets a custom title for the card. | string | `WakaTime Stats` |
| `layout` | Switches between two available layouts `default` & `compact`. | enum | `default` |
| `langs_count` | Limits the number of languages on the card, defaults to all reported languages. | integer | `null` |
| `api_domain` | Sets a custom API domain for the card, e.g. to use services like [Hakatime](https://github.com/mujx/hakatime) or [Wakapi](https://github.com/muety/wakapi) | string | `wakatime.com` |
| `display_format` | Sets the WakaTime stats display format. Choose `time` to display time-based stats or `percent` to show percentages. | enum | `time` |
| `disable_animations` | Disables all animations in the card. | boolean | `false` |

### Demo

* Compact layout

---

# All Demos

* Default
* Hiding specific stats
* Showing additional stats
* Showing icons
* Shows GitHub logo instead rank level
* Shows user rank percentile instead of rank level
* Customize Border Color
* Include All Commits
* Themes

Choose from any of the [default themes](https://www.google.com/search?q=%23themes)

* Gradient
* Customizing stats card
* Setting card locale
* Customizing repo card
* Gist card
* Customizing gist card
* Top languages
* WakaTime card

---

## Quick Tip (Align The Cards)

By default, GitHub does not lay out the cards side by side. To do that, you can use such approaches:

### Stats and top languages cards

```html
<a href="[https://github.com/Frigg1337](https://github.com/Frigg1337)">
  <img height=200 align="center" src="[https://frigg-stats.vercel.app/api?username=Frigg1337](https://frigg-stats.vercel.app/api?username=Frigg1337)" />
</a>
<a href="[https://github.com/Frigg1337](https://github.com/Frigg1337)">
  <img height=200 align="center" src="[https://frigg-stats.vercel.app/api/top-langs?username=Frigg1337&layout=compact&langs_count=8&card_width=320](https://frigg-stats.vercel.app/api/top-langs?username=Frigg1337&layout=compact&langs_count=8&card_width=320)" />
</a>

```

### Pinning repositories

```html
<a href="[https://github.com/Frigg1337/ctf-event-tracker](https://github.com/Frigg1337/ctf-event-tracker)">
  <img align="center" src="[https://frigg-stats.vercel.app/api/pin/?username=Frigg1337&repo=ctf-event-tracker](https://frigg-stats.vercel.app/api/pin/?username=Frigg1337&repo=ctf-event-tracker)" />
</a>
<a href="[https://github.com/Frigg1337/github-readme-stats](https://github.com/Frigg1337/github-readme-stats)">
  <img align="center" src="[https://frigg-stats.vercel.app/api/pin/?username=Frigg1337&repo=github-readme-stats](https://frigg-stats.vercel.app/api/pin/?username=Frigg1337&repo=github-readme-stats)" />
</a>

```

# Deploy on your own

This instance is already deployed on **Vercel**!

## Available environment variables

GitHub Readme Stats provides several environment variables that can be used to customize the behavior of your self-hosted instance.

See [the Vercel documentation](https://vercel.com/docs/concepts/projects/environment-variables) on adding these environment variables to your Vercel instance.

> [!WARNING]
> Please remember to redeploy your instance after making any changes to the environment variables so that the updates take effect. The changes will not be applied to the previous deployments.

## Keep your fork up to date

You can keep your fork, and thus your private Vercel instance up to date with the upstream using GitHub's [Sync Fork button](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork).

# :sparkling_heart: Support the project

I open-source almost everything I can and try to reply to everyone needing help using these projects. Obviously,
this takes time. You can use this service for free.

However, if you are using this project and are happy with it or just want to encourage me to continue creating stuff, there are a few ways you can do it:

* Giving proper credit when you use github-readme-stats on your readme, linking back to it. :D
* Starring and sharing the project. :rocket:
* [](https://www.paypal.me/anuraghazra) - You can make a one-time donation via PayPal to the original author.

Thanks! :heart:

---

Contributions are welcome! <3

Made with :heart: and JavaScript.

```

```
