# 🎮 Gerenciador de Turmas para Jogos (React Native)

Este é um projeto desenvolvido durante o curso da **Rocketseat** utilizando **React Native com Expo**. A aplicação permite o gerenciamento de turmas e jogadores para jogos presenciais de forma simples e prática.

##  Funcionalidades

- ✅ Criar turmas para diferentes jogos
- ✅ Adicionar e remover jogadores por turma
- ✅ Persistência de dados local com **AsyncStorage**
- ✅ Listagem dinâmica com **FlatList**
- ✅ Validação e tratamento de erros personalizados
- ✅ Interface moderna e responsiva com **Styled Components**
- ✅ Navegação entre telas com **React Navigation**
- ✅ Estrutura de projeto escalável e componentizada
- ✅ Suporte a **modo escuro** via tema global
- ✅ Uso de **TypeScript** para segurança e tipagem estática

---

##  Telas (Screens)

- **Home**: listagem das turmas criadas
- **Nova Turma**: formulário para criar uma nova turma
- **Detalhes da Turma**: lista de jogadores por turma e opções para adicionar/remover

---

##  Tecnologias Utilizadas

| Tecnologia         | Descrição                                        |
|--------------------|--------------------------------------------------|
| React Native       | Framework principal para desenvolvimento mobile |
| Expo               | Ferramenta para desenvolvimento rápido          |
| TypeScript         | Superset do JS com tipagem estática             |
| Styled Components  | Estilização baseada em componentes              |
| AsyncStorage       | Armazenamento local (persistência offline)      |
| React Navigation   | Gerenciamento de rotas entre telas              |
| @types             | Tipagens auxiliares para bibliotecas externas   |

---

##  Organização do Projeto

```
src/
├── components/         # Componentes reutilizáveis (ex: Header, Button)
├── screens/            # Telas da aplicação (ex: Home, Players)
├── storage/            # Funções de leitura e escrita com AsyncStorage
├── theme/              # Definições de cores, fontes e estilos globais
├── utils/              # Utilitários e helpers
├── types/              # Tipagens personalizadas (@types)
└── App.tsx             # Entrada da aplicação
```

---

##  Tratamento de Erros

A aplicação conta com um sistema de **tratamento específico de exceções** usando `try/catch`, exibindo mensagens claras para o usuário quando:

- O jogador já existe na turma
- O nome da turma ou jogador está vazio
- Há erro ao salvar ou recuperar dados

---

##  Temas e Estilização

Utilizamos **Styled Components** com um tema global configurado (`ThemeProvider`). Com isso, conseguimos:

- Padronizar cores e fontes
- Alternar facilmente para tema escuro
- Estilizar componentes com base no tema

---

##  Instalação e Execução

1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/seu-repo.git
cd seu-repo
```

2. Instale as dependências

```bash
npm install
# ou
yarn
```

3. Execute com Expo

```bash
npx expo start
```

---

##  Tipagem com TypeScript

Toda a aplicação está tipada com **TypeScript**, garantindo:

- Previsibilidade de dados
- Evita bugs em tempo de desenvolvimento
- Autocompletar mais inteligente

Exemplos de tipos definidos:

```ts
export type Player = {
  name: string;
  team: string;
};

export type Group = {
  name: string;
  players: Player[];
};
```

---

##  Agradecimentos

Projeto desenvolvido com base nos ensinamentos da **Rocketseat**, utilizando práticas modernas de desenvolvimento mobile com **React Native** e **TypeScript**.

---

## 📄 Licença

Este projeto está sob a licença MIT.
