---
title: Acerca de la autenticación de dos factores
intro: '{% data reusables.two_fa.about-2fa %} Con la 2FA, tendrás que ingresar con tu nombre de usuario y contraseña y proporcionar otra forma de autenticación que solo tú sepas o a la que solo tú tengas acceso.'
redirect_from:
  - /articles/about-two-factor-authentication
  - /github/authenticating-to-github/about-two-factor-authentication
  - /github/authenticating-to-github/securing-your-account-with-two-factor-authentication-2fa/about-two-factor-authentication
versions:
  fpt: '*'
  ghes: '*'
  ghec: '*'
topics:
  - 2FA
shortTitle: Acerca de la 2FA
---

Para {% data variables.product.product_name %}, la segunda forma de autenticación es un código que es generado por una aplicación en tu dispositivo móvil{% ifversion fpt or ghec %} o enviado como mensaje de texto (SMS){% endif %}. Una vez que activas la 2FA, {% data variables.product.product_name %} genera un código de autenticación cada vez que alguien intenta iniciar sesión en tu cuenta de {% data variables.product.product_location %}. El único modo en que alguien puede iniciar sesión en tu cuenta es si conoce la contraseña y si tiene acceso al código de autenticación de tu teléfono.

{% data reusables.two_fa.after-2fa-add-security-key %}

{% ifversion fpt or ghec %}
Adicionalmente a las llaves de seguridad, también puedes utilizar {% data variables.product.prodname_mobile %} para la 2FA después de configurar una app móvil TOTP o mensajes de texto. {% data variables.product.prodname_mobile %} uses public-key cryptography to secure your account, allowing you to use any mobile device that you've used to sign in to {% data variables.product.prodname_mobile %} as your second factor.
{% endif %}

También puedes configurar métodos de recuperación adicionales en caso de que pierdas el acceso a tus credenciales de autenticación de dos factores. Para obtener más información acerca de la configuración de la 2FA, consulta "[Configurar autenticación de dos factores](/articles/configuring-two-factor-authentication)" y "[Configurar métodos de recuperación de autenticación de dos factores](/articles/configuring-two-factor-authentication-recovery-methods)".

Te recomendamos **enfáticamente** que habilites la 2FA para mantener la seguridad de tu cuenta, no solo en {% data variables.product.product_name %}, sino en otros sitios web y aplicaciones que la admitan. Puedes habilitar la 2FA para acceder a {% data variables.product.product_name %} y a {% data variables.product.prodname_desktop %}.

Para obtener más información, consulta "[Acceder a {% data variables.product.prodname_dotcom %} utilizando autenticación de dos factores](/articles/accessing-github-using-two-factor-authentication)".

## Códigos de recuperación de autenticación de dos factores

{% data reusables.two_fa.about-recovery-codes %} Para obtener más información, consulta "[Recuperar tu cuenta si pierdes tus credenciales 2FA](/articles/recovering-your-account-if-you-lose-your-2fa-credentials)".

{% ifversion fpt or ghec %}

{% warning %}

**Advertencia**: {% data reusables.two_fa.support-may-not-help %} Para obtener más información, consulta "[Recuperar tu cuenta si pierdes tus credenciales 2FA](/articles/recovering-your-account-if-you-lose-your-2fa-credentials)".

{% endwarning %}

{% endif %}

## Solicitar autenticación de dos factores en tu organización

Los propietarios de la organización pueden solicitar que los miembros{% ifversion fpt or ghec %} de la organización, los gerentes de facturación, {% endif %} y los colaboradores externos usen la autenticación de dos factores para proteger sus cuentas personales. Para obtener más información, consulta "[Solicitar la autenticación de dos factores en tu organización](/articles/requiring-two-factor-authentication-in-your-organization)".

{% data reusables.two_fa.auth_methods_2fa %}
