# Integrando a Carta de Serviços Eletrônica com o portal Institucional do Órgão

A integração é realizada a partir da Barra Brasil mostrada na Figura abaixo. O objetivo é fazer com que o cidadão acesse a Carta de Serviços Eletrônica diretamente ao selecionar a opção “Serviços” na Barra Brasil presente no portal institucional do órgão. Sendo assim, o contexto da navegação será mantido.

![](imagens/barra-brasil.png)
Figura 12: Barra Brasil

Para isso, basta realizar o seguinte procedimento:

1. Inserir no código html do site institucional a meta tag “creator.productor” com o identificador do órgão no Sistema de Informações Organizacionais – SIORG;
2. A barra ser chamada após a meta tag conforme manual disponível em http://barra.governoeletronico.gov.br/.

Uma página funcional para teste pode ser vista em barra.governoeletronico.gov.br/teste/

Cada órgão deve procurar o seu código no site do SIORG disponível no endereço https://siorg.planejamento.gov.br/siorg-cidadao-webapp/pages/listar_orgaos_estruturas/listar_orgaos_estruturas.jsf Abaixo segue um exemplo de código html adicionado na página com a tag requerida em destaque apontando para o id do Ministério do Planejamento (2981).

        <!DOCTYPE html>
        <html lang="pt-BR">
        <head>
                  <meta charset="utf-8" />
                  <meta name=viewport content="width=device-width, initial-scale=1">
                  <meta property="creator.productor" content="http://estruturaorganizacional.dados.gov.br/id/unidade-organizacional/2981"/>
       <title>Barra Brasil</title>