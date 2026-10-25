# IRIDIUM Cloud para iOS

Launcher nativo en SwiftUI con estética de consola, mando Bluetooth y secciones Juego, Biblioteca, Cuentas y Configuración. La biblioteca empieza vacía; no incluye juegos de ejemplo ni tiendas de PC.

## Generar un IPA en GitHub

Subi el contenido de outputs a la raiz del repo. Ejecuta Actions y corre Build signed iOS IPA. project.yml genera Xcode con XcodeGen.
- IOS_CERTIFICATE_P12_BASE64: certificado Apple Development p12 en Base64.
- IOS_CERTIFICATE_PASSWORD: contraseña del certificado.
- IOS_PROVISIONING_PROFILE_BASE64: perfil mobileprovision en Base64.
- IOS_TEAM_ID: identificador de equipo Apple Developer.

Definí también la variable IOS_BUNDLE_ID para que coincida con el perfil. El IPA se descarga desde el artefacto IRIDIUMCloud-IPA. El perfil de desarrollo debe incluir el iPhone de destino.

## Login y lanzamiento
Cada tarjeta abre el servicio oficial y este administra el inicio de sesión. La biblioteca queda vacía hasta integrar catálogos autorizados; el lanzamiento directo por juego depende de enlaces profundos que los proveedores no ofrecen de forma uniforme en iOS. GeForce NOW y Xbox documentan su experiencia de iPhone mediante Safari, así que la app nativa entrega el control al proveedor en vez de mostrar un navegador propio.

Fuentes: https://www.nvidia.com/en-us/geforce-now/faq/ y https://www.xbox.com/en-us/xbox-on-mobile

Referencia visual independiente; no incluye emulación ni código copiado de Iridium.
