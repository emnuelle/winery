👥 Integrantes
Emanuelle Soares  —  RM97973
Julia Amorim  —  RM99609

👨‍🏫 Professor
Carlos Eduardo Machado de Oliveira

# 🍷 WinerySys - Sistema de Web Services SOAP

Projeto desenvolvido como parte do **Checkpoint 2** da disciplina **Arquitetura SOA e Web Services** (FIAP), com o objetivo de aplicar conceitos de integração entre serviços utilizando a tecnologia SOAP.

## 🎯 Objetivo

Criar uma aplicação SOAP com dois Web Services distintos:

- **WineStockService**: expõe métodos de catálogo e pedido de vinhos.
- **WineWarningService**: fornece alertas de estoque insuficiente.

A aplicação foi construída com **Java 17**, utilizando o **JAX-WS** via **Maven**, e publicada localmente via `Endpoint.publish`.

---

## 🚀 Como executar o projeto

### ✅ Pré-requisitos

- Java JDK 17+
- Apache Maven 3.8+
- IntelliJ IDEA (ou outro IDE compatível com Maven)

### 📦 Instalação e build

1. Clone o repositório:

```bash
git clone https://github.com/seu-usuario/WinerySys.git
cd WinerySys/Publisher/WinerySys

    Compile e baixe as dependências:

mvn clean install

    Execute a classe Loader.java:

        Dentro da IDE: clique com o botão direito > Run Loader.main()

        Ou, via terminal:

mvn exec:java -Dexec.mainClass="br.com.fiap.winery.Loader"

🌐 Endpoints SOAP expostos
Serviço	URL para WSDL
WineStockService	http://localhost:8085/WineStockService?wsdl

WineWarningService	http://localhost:8086/WineWarningService?wsdl
📂 Estrutura do Projeto

WinerySys/
├── pom.xml
└── src/
    └── main/
        └── java/
            └── br/
                └── com/
                    └── fiap/
                        └── winery/
                            ├── Loader.java
                            ├── WineStockService.java
                            ├── WineStockServiceImplementation.java
                            ├── WineWarningService.java
                            └── WineWarningServiceImplementation.java

