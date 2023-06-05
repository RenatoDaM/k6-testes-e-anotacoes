# Tipos de teste de carga
#
- <b>Smoke Tests</b> -> Verifica se seu script funciona de forma correta e seu sistema performa adequadamente em capacidades mínimas.


- <b>Average-load Test</b> -> Verifica como seu sistema irá performar em condições normais e esperadas.


- <b>Stress Tests</b> -> Verifica como seu sistema irá performar quando a capacidade excede o esperado.


- <b>Soak Tests</b> -> Verifica a capacidade do seu sistema de manter o desempenho ao longo de períodos extensos.


- <b>Spike Tests </b> -> Valida o comportamento e a capacidade do seu sistema sobreviver a casos de aumento repentivo, breve e massivos na atividade.


- <b>Breakpoint Tests</b> -> Gradualmente aumenta a a carga para identificar o limites de capacidade do seu sistema.

####  A seguinte tabela foi retirada da [documentação oficial do K6](https://k6.io/docs/test-types/) 

<table><thead><tr><th>Type</th><th>VUs/Throughput</th><th>Duration</th><th>When?</th></tr></thead><tbody><tr><td>Smoke</td><td>Low</td><td>Quick (seconds or minutes)</td><td>Every time new code or a change is done. It checks scripts, baseline system metrics, and deviations from changes</td></tr><tr><td>Load</td><td>Average production</td><td>Mid (15-60 minutes)</td><td>Often to check system maintains performance with average use</td></tr><tr><td>Stress</td><td>High (above average)</td><td>Mid (15-60 minutes)</td><td>When system may receive above-average loads to check how it manages</td></tr><tr><td>Soak</td><td>Average</td><td>Long (hours)</td><td>After changes to check system under prolonged continuous use</td></tr><tr><td>Spike</td><td>Very high</td><td>Quick (seconds to minutes)</td><td>Rarely, when system risks sudden rush</td></tr><tr><td>Breakpoint</td><td>Increases until break</td><td>As long as necessary</td><td>A few times to find the upper limits of the system</td></tr></tbody></table>


## Recomendações gerais

- Comece com um <b>smoke test</b>.
- A carga de testes pode variar muito dependendo de cada sistema.
- Não tem nenhum teste que te garante cobertura em tudo. São necessários vários tipos de teste.