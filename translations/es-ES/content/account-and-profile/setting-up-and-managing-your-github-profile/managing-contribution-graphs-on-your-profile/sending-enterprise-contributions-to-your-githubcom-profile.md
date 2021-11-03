---
title: Enviar contribuciones empresariales a tu perfil de GitHub.com
intro: 'Puedes resaltar tu trabajo en {% data variables.product.prodname_enterprise %} al enviar los recuentos de contribuciones a tu perfil {% data variables.product.prodname_dotcom_the_website %}.'
redirect_from:
  - /articles/sending-your-github-enterprise-contributions-to-your-github-com-profile/
  - /articles/sending-your-github-enterprise-server-contributions-to-your-github-com-profile
  - /articles/sending-your-github-enterprise-server-contributions-to-your-githubcom-profile
  - /github/setting-up-and-managing-your-github-profile/sending-your-github-enterprise-server-contributions-to-your-githubcom-profile
  - /github/setting-up-and-managing-your-github-profile/managing-contribution-graphs-on-your-profile/sending-your-github-enterprise-server-contributions-to-your-githubcom-profile
versions:
  fpt: '*'
  ghes: '*'
  ghae: next
  ghec: '*'
topics:
  - Profiles
shortTitle: Enviar contribuciones empresariales
---

## Acerca de las contribuciones empresariales en tu perfil de {% data variables.product.prodname_dotcom_the_website %}

Your {% data variables.product.prodname_dotcom_the_website %} profile shows {% ifversion fpt or ghec %}{% data variables.product.prodname_ghe_server %}{% ifversion ghae-next %}<!-- Remove condition entirely when toggling feature flag --> or {% data variables.product.prodname_ghe_managed %}{% endif %}{% else %}{% data variables.product.product_name %}{% endif %} contribution counts from the past 90 days. Los recuentos de contribuciones de {% data reusables.github-connect.sync-frequency %} de {% data variables.product.prodname_enterprise %} se consideran contribuciones privadas. Los detalles de confirmación solo mostrarán los conteos de contribuciones y que estas se hicieron en un ambiente de {% data variables.product.prodname_enterprise %} fuera de {% data variables.product.prodname_dotcom_the_website %}.

Puedes decidir si quieres que se muestren los conteos de las contribuciones privadas en tu perfil. Para obtener más información, consulta "[Publicar u ocultar tus contribuciones privadas en tu perfil](/articles/publicizing-or-hiding-your-private-contributions-on-your-profile/)."

Para obtener más información acerca de cómo se calculan las contribuciones, consulta "[Administrar gráficos de contribuciones en tu perfil](/articles/managing-contribution-graphs-on-your-profile/)."

{% note %}

**Notas:**
- La conexión entre tus cuentas está regulada por la <a href="/articles/github-privacy-statement/" class="dotcom-only">Declaración de privacidad de GitHub</a>, y los usuarios que habilitan la conexión aceptan los Términos de servicio de GitHub<a href="/articles/github-terms-of-service/" class="dotcom-only"></a>.

- Before you can connect your {% ifversion fpt or ghec %}{% data variables.product.prodname_ghe_server %}{% ifversion ghae-next %}<!-- Remove condition entirely when toggling feature flag --> or {% data variables.product.prodname_ghe_managed %}{% endif %}{% else %}{% data variables.product.product_name %}{% endif %} profile to your {% data variables.product.prodname_dotcom_the_website %} profile, your enterprise owner must enable {% data variables.product.prodname_github_connect %} and enable contribution sharing between the environments. Para obtener más información, contacta a tu propietario de empresa.

{% endnote %}

{% ifversion fpt or ghes or ghae or ghec %}

## Enviar las contribuciones de tu empresa a tu perfil de {% data variables.product.prodname_dotcom_the_website %}

{% ifversion fpt or ghec %}

- Para enviar contribuciones empresariales desde {% data variables.product.prodname_ghe_server %} a tu perfil de {% data variables.product.prodname_dotcom_the_website %}, consulta la sección "[Enviar contribuciones empresariales a tu perfil de {% data variables.product.prodname_dotcom_the_website %}](/enterprise-server/account-and-profile/setting-up-and-managing-your-github-profile/managing-contribution-graphs-on-your-profile/sending-enterprise-contributions-to-your-githubcom-profile)" en la documentación de {% data variables.product.prodname_ghe_server %}.{% ifversion ghae-next %}<!-- Condition is within an fpt block; remove condition entirely when toggling feature flag -->
- Para enviar contribuciones empresariales desde {% data variables.product.prodname_ghe_managed %} a tu perfil de {% data variables.product.prodname_dotcom_the_website %}, consulta la sección "[Enviar contribuciones empresariales a tu perfil de {% data variables.product.prodname_dotcom_the_website %}](/github-ae@latest/account-and-profile/setting-up-and-managing-your-github-profile/managing-contribution-graphs-on-your-profile/sending-enterprise-contributions-to-your-githubcom-profile)" en la documentación de {% data variables.product.prodname_ghe_managed %}.{% endif %}

{% elsif ghes %}

1. Iniciar sesión en {% data variables.product.prodname_ghe_server %} y {% data variables.product.prodname_dotcom_the_website %}.
1. En {% data variables.product.prodname_ghe_server %}, en la esquina superior derecha de cualquier página, haz clic en tu foto de perfil y luego haz clic en **Ajustes**. ![Icono Settings (Parámetros) en la barra de usuario](/assets/images/help/settings/userbar-account-settings.png)
{% data reusables.github-connect.github-connect-tab-user-settings %}
{% data reusables.github-connect.connect-dotcom-and-enterprise %}
1. Revisa los recursos a los que {% data variables.product.prodname_ghe_server %} accederá desde tu cuenta de {% data variables.product.prodname_dotcom_the_website %}, posteriormente, da clic en **Autorizar**. ![Autorizar conexión entre GitHub Enterprise Server y GitHub.com](/assets/images/help/settings/authorize-ghe-to-connect-to-dotcom.png)
{% data reusables.github-connect.send-contribution-counts-to-githubcom %}

{% elsif ghae %}

1. Iniciar sesión en {% data variables.product.prodname_ghe_managed %} y {% data variables.product.prodname_dotcom_the_website %}.
1. En {% data variables.product.prodname_ghe_managed %}, en la esquina superior derecha de cualquier página, haz clic en tu foto de perfil y luego haz clic en **Ajustes**. ![Icono Settings (Parámetros) en la barra de usuario](/assets/images/help/settings/userbar-account-settings.png)
{% data reusables.github-connect.github-connect-tab-user-settings %}
{% data reusables.github-connect.connect-dotcom-and-enterprise %}
{% data reusables.github-connect.authorize-connection %}
{% data reusables.github-connect.send-contribution-counts-to-githubcom %}

{% endif %}

{% endif %}