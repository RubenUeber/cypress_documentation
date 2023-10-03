# cypress_documentation
Documento de guia do Cypress


>>>Boas práticas para documentação de relatório dos testes

1 - No terminal, instalar o mochawesome para executar as gravações em um determinado diretório.
Use o seguinte comando:
npm install --save-dev mochawesome

2 - Em seguida, abra o cypress.config.js e, após module.exports = defineConfig({ e2e: {,
cole o seguinte código:
 setupNodeEvents(on, config) {
                { "reporter"; "mochawesome",
                    "reporterOptions"; 
                        { "reportDir"; "cypress/report/mochawesome-report",
                        "overwrite"; true,
                        "html"; true,
                        "json"; true,
                        "timestamp"; "mmddyyyy_HHMMss" }}

3 - Em seguida rode o comando no terminal, npm install --save-dev mochawesome


