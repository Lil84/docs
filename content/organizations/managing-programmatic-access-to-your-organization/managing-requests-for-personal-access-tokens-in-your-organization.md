---
title: Managing requests for personal access tokens in your organization
intro: 'Organization owners can approve or deny {% data variables.product.pat_v2 %}s that request access to their organization.'
versions:
  feature: pat-v2
shortTitle: Manage token requests
---

{% data reusables.user-settings.pat-v2-org-opt-in %}

## About {% data variables.product.pat_v2 %} requests

When organization members create a {% data variables.product.pat_v2 %} to access resources owned by the organization, if the organization requires approval for {% data variables.product.pat_v2 %}s, then an organization owner must approve the token before it can be used to access any resources that are not public. For more information, see "[Setting a {% data variables.product.pat_generic %} policy for your organization](/organizations/managing-programmatic-access-to-your-organization/setting-a-personal-access-token-policy-for-your-organization)."

{% data variables.product.company_short %} will notify organization owners with a daily email about all {% data variables.product.pat_v2 %}s that are awaiting approval. When a token is denied or approved, the user who created the token will receive an email notification.

{% note %}

**Note**: Only {% data variables.product.pat_v2 %}s, not {% data variables.product.pat_v1_plural %}, are subject to approval. Unless the organization has restricted access by {% data variables.product.pat_v1_plural %}, any {% data variables.product.pat_v1 %} can access organization resources without prior approval. For more information, see "[Setting a {% data variables.product.pat_generic %} policy for your organization](/organizations/managing-programmatic-access-to-your-organization/setting-a-personal-access-token-policy-for-your-organization)."

{% endnote %}

## Managing {% data variables.product.pat_v2 %} requests

{% data reusables.profile.access_org %}
{% data reusables.profile.org_settings %}
1. In the left sidebar, under **{% octicon "key" aria-label="The key icon" %} {% data variables.product.pat_generic_caps %}s**, click **Pending requests**. If any tokens are pending approval for your organization, they will be displayed.
1. Click the name of the token that you want to approve or deny.
1. Review the access and permissions that the token is requesting.
1. To grant the token access to the organization, click **Approve**. To deny the token access to the organization, click **Deny**.
1. If you denied the request, in the confirmation box, optionally enter the reason that you denied the token. This reason will be shared in the notification that is sent to the token owner. Then, click **Deny**.

Alternatively, you can approve or deny multiple tokens at once:

{% data reusables.profile.access_org %}
{% data reusables.profile.org_settings %}
1. In the left sidebar, under **{% octicon "key" aria-label="The key icon" %} {% data variables.product.pat_generic_caps %}s**, click **Pending requests**. If any tokens are pending approval for your organization, they will be displayed.
1. Optionally, use the **Owner** and **Repository** dropdown menus to filter the requests by the member making the request.
1. Select each token that you want to approve or reject.
1. Select the **request selected...** dropdown menu and click **Approve...** or **Deny...**.
