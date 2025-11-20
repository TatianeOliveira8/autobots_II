# AutoBots - Gestão das Lojas Especializadas em Manutenção Veicular

## Estrutura e funcionalidades

O AutoBots é um sistema voltado para gerenciamento de clientes, documentos, telefones e endereços de lojas de manutenção veicular e vendas de autopeças.  

Funcionalidades principais:  
- CRUD completo de clientes, documentos, telefones e endereços.  
- Implementação dos **níveis de maturidade RMM.  
- Arquitetura seguindo princípios **SOLID**.

---

### 📝 Rotas disponíveis

#### **CLIENTE:**
- **GET** `http://localhost:8080/clientes` - Lista todos  
- **GET** `http://localhost:8080/cliente/{id}` - Busca por ID  
- **POST** `http://localhost:8080/cliente/cadastro` - Criar  
- **PUT** `http://localhost:8080/cliente/atualizar` - Atualizar  
- **DELETE** `http://localhost:8080/cliente/excluir` - Excluir  

#### **DOCUMENTO:**
- **GET** `http://localhost:8080/documentos` - Lista todos  
- **GET** `http://localhost:8080/documento/{id}` - Busca por ID  
- **POST** `http://localhost:8080/documento/cadastro` - Criar  
- **PUT** `http://localhost:8080/documento/atualizar` - Atualizar  
- **DELETE** `http://localhost:8080/documento/excluir` - Excluir  

#### **TELEFONE:**
- **GET** `http://localhost:8080/telefones` - Lista todos  
- **GET** `http://localhost:8080/telefone/{id}` - Busca por ID  
- **POST** `http://localhost:8080/telefone/cadastro` - Criar  
- **PUT** `http://localhost:8080/telefone/atualizar` - Atualizar  
- **DELETE** `http://localhost:8080/telefone/excluir` - Excluir  

#### **ENDEREÇO:**
- **GET** `http://localhost:8080/enderecos` - Lista todos  
- **GET** `http://localhost:8080/endereco/{id}` - Busca por ID  
- **POST** `http://localhost:8080/endereco/cadastro` - Criar  
- **PUT** `http://localhost:8080/endereco/atualizar` - Atualizar  
- **DELETE** `http://localhost:8080/endereco/excluir` - Excluir  

---

## Exemplo de JSON para teste rápido (cliente)

```json
{
  "nome": "Maria Souza",
  "nomeSocial": "Maria",
  "dataNascimento": "1985-03-10",
  "dataCadastro": "2025-11-20",
  "documentos": [
    {
      "tipo": "CPF",
      "numero": "987.654.321-00"
    }
  ],
  "endereco": {
    "estado": "RJ",
    "cidade": "Rio de Janeiro",
    "bairro": "Copacabana",
    "rua": "Avenida Atlântica",
    "numero": "1702",
    "codigoPostal": "22021-001"
  },
  "telefones": [
    {
      "ddd": "21",
      "numero": "99876-5432"
    }
  ]
}
````

---

## Ambiente de Teste

* **Java:** 17
* **Framework:** Spring Boot
* **IDE:** VS Code
