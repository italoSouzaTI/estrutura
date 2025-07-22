-src
|\_core
-Chamada principais da API
-Criação de banco de dados ou storage
-Thema padrão do aplicativo
|\_features estrutura(MVVM)
-Divisão de telas por pasta

     -Ex.: Home
                |_API chamas.
                |_Hooks especificos de lógica de negocios quebradas em partes.
                |_Components especificos dessa tela.
                |_useModelView lógica de negocios.
                |_Home.tsx ou index.tsx - Recomendo coloca nome da pasta na tela para index tudo no index.ts da features
                |_styles.ts

    |\_routes : criando rotas caso use react navigation se usar o expo-route e outra estrutura.

    |\_shared : Criação de componentes sem amarração de lógica com components, helps,hooks e service global.

    |\_store : pode ser usando context ou zustand ou redux para controla estados da aplicação como um todo ou podento criar uma propria store dentro de features ou das subpastas para controlas micro ciclos internos.
