# Documentação do Projeto: **TaskComplete**

## Visão Geral

Este projeto é uma aplicação Android construída com **Jetpack Compose**, visando proporcionar uma interface simples para exibir uma tela de "tarefa concluída". A tela apresenta uma imagem e duas mensagens de texto indicando que todas as tarefas foram concluídas com sucesso. Este projeto é um exemplo de uso do **Material3** para a construção de interfaces modernas no Android.

O código foca em demonstrar como trabalhar com `Image` e `Text` composables, alinhando elementos centralizados na tela, e utilizando recursos de string e imagens para facilitar a internacionalização e a reutilização de componentes.

## Funcionalidade

Quando o aplicativo é iniciado, ele exibe:
- Uma imagem de conclusão de tarefa.
- Uma mensagem indicando que todas as tarefas foram completadas.
- Uma mensagem de agradecimento ou incentivo.

Essa interface pode ser utilizada, por exemplo, em um aplicativo de gerenciamento de tarefas ou como uma tela final de algum processo.

### Layout da Interface

A tela é composta da seguinte estrutura:
- **Imagem**: Uma imagem representando a conclusão de uma tarefa, que é exibida no centro da tela.
- **Texto**: Duas mensagens textuais:
  - "All tasks completed" (todas as tarefas foram concluídas).
  - "Nice work!" (bom trabalho!).

As mensagens são centralizadas e apresentadas com um espaçamento adequado para uma boa legibilidade.

### Composables Utilizados

- **Column**: Usado para organizar os elementos de forma vertical.
- **Row**: Usado para organizar a imagem e os textos de maneira horizontal, quando necessário.
- **Image**: Exibe a imagem de conclusão de tarefa.
- **Text**: Exibe as mensagens de texto.
- **stringResource**: Utilizado para acessar as strings definidas no arquivo de recursos `strings.xml`, permitindo a internacionalização do aplicativo.
- **painterResource**: Usado para carregar a imagem da pasta de recursos `drawable`.

## Estrutura do Código

### MainActivity.kt

- **onCreate()**: Método responsável por configurar a atividade e definir o conteúdo da tela. A função `taskComplete()` é chamada dentro de um `Scaffold` para gerar o layout da tela.
- **taskComplete()**: Função composable que cria a estrutura da interface. Ela utiliza `Column` para organizar verticalmente os elementos na tela e `Row` para alinhar as imagens e textos.
- **Text()**: Exibe as mensagens de texto, com estilização como peso de fonte e tamanho da fonte.
- **Image()**: Exibe uma imagem (ícone) de tarefa concluída, carregada de um arquivo no diretório de recursos.
- **Scaffold**: Usado como estrutura para o layout, permitindo adicionar padding e gerenciar a tela de forma mais eficiente.

### Recursos

- **strings.xml**: Contém as mensagens de texto usadas no aplicativo, facilitando a internacionalização.
  - `all_tasks_completed`: Mensagem de confirmação de tarefas concluídas.
  - `nice_work`: Mensagem de agradecimento.

- **ic_task_completed.png**: A imagem usada para representar a conclusão das tarefas, localizada no diretório `res/drawable`.

## Dependências

Não há dependências externas específicas além do uso do **Jetpack Compose** e **Material3** que já fazem parte do SDK Android para desenvolvimento de interfaces de usuário modernas.

- **Jetpack Compose**: Framework para a criação de interfaces de usuário de forma declarativa.
- **Material3**: Biblioteca de componentes para a criação de interfaces com base nas diretrizes de design do Google.

## Como Rodar o Projeto

1. **Instalar o Android Studio**: Certifique-se de ter o [Android Studio](https://developer.android.com/studio) instalado no seu computador.
2. **Clonar o Repositório**: Clone este repositório para o seu ambiente local.
3. **Abrir o Projeto**: Abra o projeto no Android Studio.
4. **Executar o Projeto**: Conecte um dispositivo Android ou use um emulador para executar o aplicativo.

## Conclusão

Este projeto foi desenvolvido como uma demonstração simples do uso de **Jetpack Compose** e **Material3** para criar uma interface de usuário agradável e funcional em um aplicativo Android. Ele é útil como exemplo de como exibir uma tela simples de confirmação de tarefa ou de finalização de algum processo, e serve como base para a construção de interfaces de usuários mais complexas em projetos futuros.
