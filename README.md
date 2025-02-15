[![Node.js CI](https://github.com/jfoclpf/in-my-district/actions/workflows/android.yml/badge.svg)](https://github.com/jfoclpf/in-my-district/actions/workflows/android.yml)
[![Node.js CI](https://github.com/jfoclpf/in-my-district/actions/workflows/ios.yml/badge.svg)](https://github.com/jfoclpf/in-my-district/actions/workflows/ios.yml)
[![js-standard-style][js-standard-style_img]][js-standard-style_url]
[![Total alerts](https://img.shields.io/lgtm/alerts/g/jfoclpf/in-my-district.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/jfoclpf/in-my-district/alerts/)
[![Language grade: JavaScript](https://img.shields.io/lgtm/grade/javascript/g/jfoclpf/in-my-district.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/jfoclpf/in-my-district/context:javascript)
<br>
[![Donate with librepay](https://img.shields.io/liberapay/receives/joaopimentel1980.svg?logo=liberapay)](https://en.liberapay.com/joaopimentel1980)
[![Donate with librepay](https://img.shields.io/badge/donate-Donate-yellow?logo=liberapay)](https://en.liberapay.com/joaopimentel1980/donate)

[js-standard-style_img]: https://img.shields.io/badge/code%20style-standard-brightgreen.svg
[js-standard-style_url]: https://standardjs.com/

# No meu bairro!

Aplicação móvel para comunicar ao seu Município e/ou Junta de Freguesia anomalias no seu bairro, como buracos na calçada ou lixo por recolher.

O código está desenhado em Javascript para ser corrido num smartphone. Para tal faz uso da plataforma <a href="https://cordova.apache.org/">Apache Cordova</a>.

* A APP para Android está aqui : <a href="https://f-droid.org/packages/com.in.my.district/">F-Droid</a>, <a href="https://play.google.com/store/apps/details?id=com.in.my.district">Google Play</a>

## Estrutura

Este repositório contém o código de três componentes principais, contidos nas seguintes diretorias:

 - [`app/`](app/): Aplicação móvel para Android ou iOS, escrita em Apache Cordova (Javascript)
 - [`server/`](server/): Servidor em NodeJS para comunicar com a APP e com uma base de dados MySQL
 - [`website/`](website/): Página web desenvolvida em Wordpress para anunciar o projeto e publicar as ocorrências

## Como instalar e testar a APP
### Requisitos, _debug_ e eventuais problemas

* ver [documentação](https://github.com/jfoclpf/in-my-district/blob/master/docs.md)

### Android

 1. Clone este projeto<br>`git clone https://github.com/jfoclpf/in-my-district.git`
 2. Entre na pasta recém criada<br>`cd in-my-district/app`
 3. Adicione a plataforma<br>`cordova platform add android`
 3. Corra `cordova build android` para construir o projeto na sua máquina. Em Android cria o ficheiro APK na pasta `platforms/android/build/outputs/apk`

### iOS
```
git clone https://github.com/jfoclpf/in-my-district.git
cd in-my-district/app
cordova platform rm android
cordova platform add ios
open platforms/ios/No\ meu\ Bairro\!.xcworkspace/
```

## Contribuições são muito bem-vindas

 * Usamos StandardJS para o código
 * Respeite a estrutura dos ficheiros
 * Comente sempre o código (preferencialmente em Inglês), tal ajuda os outros a compreender as suas contribuiçes

## Licença

[GNU GPLv3](http://www.gnu.org/licenses/gpl-3.0.en.html)
