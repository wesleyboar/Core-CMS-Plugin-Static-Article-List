## Texas Advanced Computing Center
# Django CMS Plugin: "Article List (Static)"

This plugin renders a static list of article previews.

- __`__dist-name__`__: `djangocms-tacc-static-article-list`
- __`__package_name__`__: `djangocms_tacc_static_article_list`
- __`__ClassName__`__: `TaccsiteArticleList`
- __"Plugin Name"__: "Article List (Static)"

<details><summary>Intent</summary>

_This plugin only exists because of the unavailaibility of a solution to sync news between two TACC websites. To learn more, see [TACC/Core-CMS wiki page "Static-Article-Plugins"][tacc-sa-plugins]._

</details>

## Quick Start

1. Follow https://github.com/tacc-wbomar/Core-CMS-Plugin/wiki/Core-CMS-Plugin-Usage-Quick-Start.

## Usage

1. Add instance of plugin to a page.
1. Configure the plugin instance.
1. Add instance(s) of [`djangocms_tacc_static_article_preview`][tacc-sa-preview] within this plugin.
1. See plugin render content that matches configuration.

## Features

1. Render a list container, optionally with title and/or "See All" link.
2. Renders supported, nested plugin instances of [`djangocms_tacc_static_article_preview`][tacc-sa-preview].
    <details>

    | kind | description |
    | :- | :- |
    | News | [external news articles][tacc-sa-plugins] |
    | Documents | [single-topic documents][tacc-core-docs] |
    | Allocations | [date range for applications][fp-allocs] |
    | Events | [learning opportunities][tacc-learn] |

    </details>
3. Uses supported, integrated plugin instances to incorporate extra features.
    <details>

    | feature | supported by |
    | :- | :- |
    | a "See All" hyperlink | [`djangocms_tacc_data_list`][dcms-link] |

    </details>

## Caveats

1. Requires [`djangocms_link`][dcms-link].\*

> \* Support is optional but plugin is assummed, so plugin is required. This could change in a future release.



[fp-allocs]: https://frontera-portal.tacc.utexas.edu/allocations/

[tacc-learn]: https://learn.tacc.utexas.edu/
[tacc-core-docs]: https://cep.tacc.utexas.edu/guides/
[tacc-sa-plugins]: https://github.com/TACC/Core-CMS/wiki/Static-Article-Plugins
[tacc-sa-preview]: https://github.com/tacc-wbomar/Core-CMS-Plugin-Static-Article-Preview
