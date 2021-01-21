# Gerador de contatos
Essa página foi criada para facilitar um experimento: o que acontece se você criar um grupo de Whatsapp com todos as pessoas (que tem Whatsapp!) que tem o mesmo número de celular, mas em diferentes DDDs.

Ao digitar seu número de celular com DDD no campo indicado, a porção em JavaScript da página gera um arquivo .vcf com os contatos com o mesmo número porém de DDD diferente do original. A lista de DDDs foi gerada [a partir da lista de DDDs da Wikipedia](https://pt.wikipedia.org/wiki/Discagem_direta_a_dist%C3%A2ncia#Lista_de_c%C3%B3digos_DDD_brasileiros_por_estado,_com_as_principais_cidades_e_regi%C3%B5es).

O arquivo .vcf tem o formato abaixo, podendo ser importado nativamente em celulares.

```
BEGIN:VCARD
VERSION:2.1
N:;12;;;
TEL;CELL:12999999999
END:VCARD
BEGIN:VCARD
VERSION:2.1
N:;13;;;
TEL;CELL:13999999999
END:VCARD
...
```

Nenhum dado do visitante é salvo, nenhum dado é enviado ao servidor e o arquivo é gerado dinamicamente por JavaScript.
