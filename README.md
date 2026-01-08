# Projeto DevOps - Pipelines CI/CD

Este repositório demonstra dois tipos de pipelines CI/CD configurados com **GitHub Actions**:

## Objetivo
Mostrar práticas de automação de testes e deploy em projetos de software, destacando diferentes estratégias de execução.

## Tipos de Pipeline

- **Fail Fast (Falha Rápida)**  
  O pipeline interrompe imediatamente ao encontrar um erro.  
  Ideal para ambientes com pouco tempo disponível, evitando desperdício de recursos.

- **Full Run (Executa até o fim)**  
  O pipeline continua rodando mesmo após falhas.  
  Útil no início do projeto, pois permite identificar todos os erros de uma vez e corrigi-los com calma.

## Estrutura dos Workflows
Cada pipeline está definido em arquivos separados dentro da pasta `.github/workflows`:
- `ci-fail-fast.yml` → Pipeline que falha rápido.  
- `ci-full-run.yml` → Pipeline que roda até o fim.

## Etapas comuns
1. **Checkout do código**  
2. **Instalação de dependências**  
3. **Testes unitários**  
4. **Testes de integração**  
5. **Build da aplicação**  
6. **Deploy (opcional)**

## Como usar
1. Faça um fork ou clone deste repositório.  
2. Ajuste os comandos de instalação e testes conforme sua linguagem (Node.js, Python, etc).  
3. Crie seus próprios jobs e personalize os workflows.  

---

✨ Este projeto serve como exemplo prático de boas práticas DevOps e pode ser expandido com monitoramento, infraestrutura como código e deploy em nuvem.
