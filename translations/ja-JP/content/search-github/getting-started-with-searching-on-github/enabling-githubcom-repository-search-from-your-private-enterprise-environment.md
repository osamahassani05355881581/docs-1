---
title: Enabling GitHub.com repository search from your private enterprise environment
shortTitle: Search GitHub.com from enterprise
intro: 'You can connect your personal accounts on {% data variables.product.prodname_dotcom_the_website %} and your private {% data variables.product.prodname_enterprise %} environment to search for content in certain {% data variables.product.prodname_dotcom_the_website %} repositories{% ifversion fpt or ghec %} from your private environment{% else %} from {% data variables.product.product_name %}{% endif %}.'
redirect_from:
  - /articles/enabling-private-githubcom-repository-search-in-your-github-enterprise-account
  - /articles/enabling-private-github-com-repository-search-in-your-github-enterprise-server-account
  - /articles/enabling-private-githubcom-repository-search-in-your-github-enterprise-server-account
  - /articles/enabling-githubcom-repository-search-in-github-enterprise-server
  - /github/searching-for-information-on-github/enabling-githubcom-repository-search-in-github-enterprise-server
  - /github/searching-for-information-on-github/getting-started-with-searching-on-github/enabling-githubcom-repository-search-in-github-enterprise-server
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
  ghec: '*'
topics:
  - GitHub search
---

## About search for {% data variables.product.prodname_dotcom_the_website %} repositories from {% ifversion fpt or ghec %}your private enterprise environment{% else %}{% data variables.product.product_name %}{% endif %}

You can search for designated private repositories on {% data variables.product.prodname_ghe_cloud %} from {% ifversion fpt or ghec %}your private {% data variables.product.prodname_enterprise %} environment{% else %}{% data variables.product.product_location %}{% ifversion ghae %} on {% data variables.product.prodname_ghe_managed %}{% endif %}{% endif %}. {% ifversion fpt or ghec %}For example, if you use {% data variables.product.prodname_ghe_server %}, you can search for private repositories from your enterprise from {% data variables.product.prodname_ghe_cloud %} in the web interface for {% data variables.product.prodname_ghe_server %}.{% endif %}

## 必要な環境

- An enterprise owner for {% ifversion fpt or ghec %}your private {% data variables.product.prodname_enterprise %} environment{% else %}{% data variables.product.product_name %}{% endif %} must enable {% data variables.product.prodname_github_connect %} and {% data variables.product.prodname_unified_search %} for private repositories. 詳しい情報については、以下を参照してください。
{% ifversion fpt %}
  - "[Enabling {% data variables.product.prodname_unified_search %} for your enterprise](/enterprise-server@latest/admin/configuration/configuring-github-connect/enabling-unified-search-for-your-enterprise)" in the {% data variables.product.prodname_ghe_server %} documentation{% endif %}{% ifversion ghec %}
  - "[Enabling {% data variables.product.prodname_unified_search %} for your enterprise](/enterprise-server@latest/admin/configuration/configuring-github-connect/enabling-unified-search-for-your-enterprise)" in the {% data variables.product.prodname_ghe_server %} documentation{% endif %}{% ifversion ghes %}
  - "[Enabling {% data variables.product.prodname_unified_search %} for your enterprise](/admin/configuration/configuring-github-connect/enabling-unified-search-for-your-enterprise)"{% endif %}{% ifversion fpt or ghec or ghae %}
  - "[Enabling {% data variables.product.prodname_unified_search %} for your enterprise](/github-ae@latest/admin/configuration/configuring-github-connect/enabling-unified-search-for-your-enterprise)"{% ifversion fpt or ghec %} in the {% data variables.product.prodname_ghe_managed %} documentation{% endif %}
{% endif %}

- You must already have access to the private repositories and connect your account {% ifversion fpt or ghec %}in your private {% data variables.product.prodname_enterprise %} environment{% else %}on {% data variables.product.product_name %}{% endif %} with your account on {% data variables.product.prodname_dotcom_the_website %}. For more information about the repositories you can search, see "[About searching on GitHub](/github/searching-for-information-on-github/getting-started-with-searching-on-github/about-searching-on-github#searching-repositories-on-githubcom-from-your-private-enterprise-environment)."

## Enabling GitHub.com repository search from {% ifversion fpt or ghec %}your private {% data variables.product.prodname_enterprise %} environment{% else %}{% data variables.product.product_name %}{% endif %}

{% ifversion fpt or ghec %}

詳しい情報については、以下を参照してください。

| Your enterprise environment                         | 詳細情報                                                                                                                                                                                                                                                                                                                                                                  |
|:--------------------------------------------------- |:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| {% data variables.product.prodname_ghe_server %}  | "[Enabling {% data variables.product.prodname_dotcom_the_website %} repository search from your private enterprise environment](/enterprise-server@latest/search-github/getting-started-with-searching-on-github/enabling-githubcom-repository-search-from-your-private-enterprise-environment#enabling-githubcom-repository-search-from-github-enterprise-server)" |
| {% data variables.product.prodname_ghe_managed %} | "[Enabling {% data variables.product.prodname_dotcom_the_website %} repository search from your private enterprise environment](/github-ae@latest//search-github/getting-started-with-searching-on-github/enabling-githubcom-repository-search-from-your-private-enterprise-environment#enabling-githubcom-repository-search-from-github-ae)"                       |

{% elsif ghes or ghae %}

1. Sign into {% data variables.product.product_name %} and {% data variables.product.prodname_dotcom_the_website %}.
1. {% data variables.product.product_name %} にあるページの右上隅でプロフィール画像をクリックしてから、[**Settings**] をクリックします。 ![ユーザバーの [Settings（設定）] アイコン](/assets/images/help/settings/userbar-account-settings.png)
{% data reusables.github-connect.github-connect-tab-user-settings %}
{% data reusables.github-connect.connect-dotcom-and-enterprise %}
{% data reusables.github-connect.connect-dotcom-and-enterprise %}

{% endif %}
