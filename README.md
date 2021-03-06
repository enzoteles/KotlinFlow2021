# KotlinFlow 2021

## Fluxos Kotlin no Android
Em corrotinas, um fluxo é um tipo que pode emitir vários valores sequencialmente, ao contrário das funções de suspensão, que retornam somente um valor. Por exemplo, você pode usar um fluxo para receber atualizações em tempo real de um banco de dados.

Os fluxos são criados com base nas corrotinas e podem fornecer vários valores. Conceitualmente, um fluxo é um stream de dados que pode ser computado de forma assíncrona. Os valores emitidos precisam ser do mesmo tipo. Por exemplo, um Flow<Int> é um fluxo que emite valores inteiros.

Um fluxo é muito semelhante a um Iterator que produz uma sequência de valores, mas usa funções de suspensão para produzir e consumir valores de maneira assíncrona. Isso significa, por exemplo, que o fluxo pode fazer uma solicitação de rede com segurança para produzir o próximo valor sem bloquear a linha de execução principal.

Há três entidades envolvidas em streams de dados:

* Um produtor produz dados que são adicionados ao stream. Graças às corrotinas, os fluxos também podem produzir dados de maneira assíncrona.
* Intermediários (opcionais) podem modificar cada valor emitido para o stream ou o próprio stream.
* Um consumidor consome os valores do stream.

<img width="646" alt="Screen Shot 2021-11-12 at 20 38 58" src="https://user-images.githubusercontent.com/5742609/141595899-8794aca5-44f1-4ee5-936f-2ab0dddc2082.png">

Exemplo de um código kotlin flow:

<img width="557" alt="Screen Shot 2021-11-12 at 20 51 31" src="https://user-images.githubusercontent.com/5742609/141596494-708f9d37-daa1-4374-a57b-9f35679fb3fe.png">

<img width="587" alt="Screen Shot 2021-11-12 at 20 51 47" src="https://user-images.githubusercontent.com/5742609/141596502-6fe8ee00-cb42-4902-a25a-6305baab1318.png">

