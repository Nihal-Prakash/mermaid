### Quicksort Algorithm

```mermaid
flowchart TB
%%Style%%
classDef green fill:#a6e22e,stroke:#000,stroke-width:2px,color:#fff
classDef pink fill:#f765af,stroke:#000,stroke-width:2px,color:#fff
classDef red fill:#db0000,stroke:#000,stroke-width:2px,color:#fff

S(Start):::green-->I(Input: Array,low,high)-->D1{Is low < high?}:::pink
D1--oY(Yes)
D1--xN(No)
N-->E(End)
Y-->P(Partion Array)-->PI[(Get Pivot Index: pi)]-->-Q(Quicksort: arr, low, pi-1)
-Q-->+Q(Quicksort: arr, pi+1, high)-->E(End):::red

