Banco API Tests

## Visão Geral do Projeto
Este projeto contém uma suíte de testes automatizados para a [Banco API](https://github.com/celiapaivab/banco-api).  
O objetivo é validar os principais endpoints da API Rest, contribuindo para qualidade e confiabilidade das operações expostas.

## Objetivos do Projeto
- Testar endpoints da API Rest de forma automatizada.  
- Verificar o correto funcionamento das operações de autenticação e transferências.  
- Gerar relatórios de execução dos testes.  

## Tecnologias e Ferramentas
O projeto utiliza as seguintes tecnologias e bibliotecas:  

- **Linguagem**: [JavaScript (Node.js)](https://nodejs.org/)  
- **Framework de Testes**: [Mocha](https://mochajs.org/)  
- **Biblioteca de Assertivas**: [Chai](https://www.chaijs.com/)  
- **Biblioteca de Requisições HTTP**: [Supertest](https://github.com/visionmedia/supertest)
- **Relatórios**: [Mochawesome](https://github.com/adamgruber/mochawesome)  
- **Gerenciamento de Váriáveis de Ambiente**: [dotenv](https://www.npmjs.com/package/dotenv)  

## Estrutura de Diretórios
```
banco-api-tests/
├── test/                 # Contém os arquivos de testes
│   ├── login.test.js
│   └── transferencias.test.js
├── mochawesome-report/   # Relatórios em HTML gerados automaticamente
├── package.json          # Dependências e scripts de execução
├── .env (não versionado) # Arquivo de variáveis de ambiente 
├── .gitignore
├── package.json          # Dependências e scripts de execução  
└── README.md
```

## Variáveis de Ambiente
Este projeto depende de um arquivo `.env` na raiz com a seguinte variável:  

```
BASE_URL=http://localhost:3000
```

- `BASE_URL`: URL base da API a ser testada (exemplo: ambiente local ou servidor remoto).  

## Como Executar
1. **Clonar o repositório**  
   ```bash
   git clone https://github.com/celiapaivab/banco-api-tests.git
   cd banco-api-tests
   ```

2. **Instalar dependências**  
   ```bash
   npm install
   ```

3. **Criar o arquivo `.env`**  
   ```bash
   echo "BASE_URL=http://localhost:3000" > .env
   ```

4. **Executar os testes**  
   ```bash
   npm test
   ```

5. **Gerar relatórios com Mochawesome**  
   Após a execução, o relatório em HTML estará disponível em:  
   ```
   ./mochawesome-report/mochawesome.html
   ```

## Documentação
- [Mocha](https://mochajs.org/)  
- [Chai](https://www.chaijs.com/)  
- [Supertest](https://github.com/visionmedia/supertest)  
- [Mochawesome](https://github.com/adamgruber/mochawesome)  
