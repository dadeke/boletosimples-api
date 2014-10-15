---
layout: reference
title: Criar Boletos - API do Boleto Simples
en: /en/reference
---

## Boletos

### POST /api/v1/bank_billets
Criar boleto

### Formatos suportados
json

### Parâmetros

<table class='table table-bordered'>
  <thead>
    <tr>
      <th>Nome do Parâmetro</th>
      <th>Descrição</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <strong>bank_billet </strong>
        <br>
        <small>
          obrigatório
        </small>
      </td>
      <td>
        Informações do Cliente
        <br>
        Value: Must be a Hash
      </td>
    </tr>

    <tr>
      <td>
        <strong>bank_billet[amount] </strong>
        <br>
        <small>
          obrigatório
        </small>
      </td>
      <td>
        Quantia (R$) - Formato: 1000,50 ou 1000.5
        <br>
        Value: Must be Float
      </td>
    </tr>

    <tr>
      <td>
        <strong>bank_billet[expire_at] </strong><br>
        <small>
          obrigatório
        </small>
      </td>
      <td>
        Data de vencimento - Formato: 31/12/2013 ou 2013-12-31
        <br>
        Value: Must be Date
      </td>
    </tr>

    <tr>
      <td>
        <strong>bank_billet[description] </strong>
        <br>
        <small>
          obrigatório
        </small>
      </td>
      <td>
        Descrição dos Serviços prestados conforme contrato.
        <br>
        Value: Must be String
      </td>
    </tr>

    <tr>
      <td>
        <strong>bank_billet[customer_person_name] </strong>
        <br>
        <small>
          obrigatório
        </small>
      </td>
      <td>
        <p>Nome ou Razão Social do Cliente</p>
        <br>
        Value: Must be String
      </td>
    </tr>

    <tr>
      <td>
        <strong>bank_billet[customer_cnpj_cpf] </strong>
        <br>
        <small>
          obrigatório
        </small>
      </td>
      <td>
        CNPJ ou CPF do Cliente
        <br>
        Value: Must be String
      </td>
    </tr>

    <tr>
      <td>
        <strong>bank_billet[customer_email] </strong>
        <br>
        <small>
          opcional
        </small>
      </td>
      <td>
        E-mail do cliente
        <br>
        Value: Must be String
      </td>
    </tr>

    <tr>
      <td>
        <strong>bank_billet[customer_address] </strong>
        <br>
        <small>
          opcional
        </small>
      </td>
      <td>
        Endereço
        <br>
        Value: Must be String
      </td>
    </tr>

    <tr>
      <td>
        <strong>bank_billet[customer_city_name] </strong>
        <br>
        <small>
          opcional
        </small>
      </td>
      <td>
        Cidade
        <br>
        Value: Must be String
      </td>
    </tr>

    <tr>
      <td>
        <strong>bank_billet[customer_state] </strong>
        <br>
        <small>
          opcional
        </small>
      </td>
      <td>
        Estado
        <br>
        Value: Must be String
      </td>
    </tr>

    <tr>
      <td>
        <strong>bank_billet[customer_neighborhood] </strong>
        <br>
        <small>
          opcional
        </small>
      </td>
      <td>
        Bairro
        <br>
        Value: Must be String
      </td>
    </tr>

    <tr>
      <td>
        <strong>bank_billet[customer_zipcode] </strong>
        <br>
        <small>
          opcional
        </small>
      </td>
      <td>
        CEP
        <br>
        Value: Must be String
      </td>
    </tr>

    <tr>
      <td>
        <strong>bank_billet[customer_address_number] </strong>
        <br>
        <small>
          opcional
        </small>
      </td>
      <td>
        Número
        <br>
        Value: Must be String
      </td>
    </tr>

    <tr>
      <td>
        <strong>bank_billet[customer_address_complement] </strong>
        <br>
        <small>
          opcional
        </small>
      </td>
      <td>
        Complemento
        <br>
        Value: Must be String
      </td>
    </tr>

    <tr>
      <td>
        <strong>bank_billet[customer_phone_number] </strong>
        <br>
        <small>
          opcional
        </small>
      </td>
      <td>
        Telefone (com DDD)
        <br>
        Value: Must be String
      </td>
    </tr>

    <tr>
      <td>
        <strong>bank_billet[customer_id] </strong>
        <br>
        <small>
          opcional
        </small>
      </td>
      <td>
        ID do Cliente Cadastrado
        <br>
        Value: Must be a number.
      </td>
    </tr>

    <tr>
      <td>
        <strong>bank_billet[notification_url] </strong>
        <br>
        <small>
          opcional
        </small>
      </td>
      <td>
        URL de notificação para onde serão enviadas notificações nas mudanças de status do boleto
          <br>
          Value: Must be String
        </td>
      </tr>

      <tr>
        <td>
          <strong>bank_billet[send_email_on_creation] </strong>
          <br>
          <small>
            opcional
          </small>
        </td>
        <td>
          Enviar por email
          <br>
          Value: Must be &#39;true&#39; or &#39;false&#39;
        </td>
      </tr>
    </tbody>
  </table>