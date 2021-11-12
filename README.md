# KotlinFlow 2021

## Fluxos Kotlin no Android
Em corrotinas, um fluxo é um tipo que pode emitir vários valores sequencialmente, ao contrário das funções de suspensão, que retornam somente um valor. Por exemplo, você pode usar um fluxo para receber atualizações em tempo real de um banco de dados.

Os fluxos são criados com base nas corrotinas e podem fornecer vários valores. Conceitualmente, um fluxo é um stream de dados que pode ser computado de forma assíncrona. Os valores emitidos precisam ser do mesmo tipo. Por exemplo, um Flow<Int> é um fluxo que emite valores inteiros.

Um fluxo é muito semelhante a um Iterator que produz uma sequência de valores, mas usa funções de suspensão para produzir e consumir valores de maneira assíncrona. Isso significa, por exemplo, que o fluxo pode fazer uma solicitação de rede com segurança para produzir o próximo valor sem bloquear a linha de execução principal.

Há três entidades envolvidas em streams de dados:

* Um produtor produz dados que são adicionados ao stream. Graças às corrotinas, os fluxos também podem produzir dados de maneira assíncrona.
* Intermediários (opcionais) podem modificar cada valor emitido para o stream ou o próprio stream.
* Um consumidor consome os valores do stream.




